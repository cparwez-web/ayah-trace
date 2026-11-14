# Ayah Trace: how to put it online and install it

The app is a plain website (no server, no build step). Upload this folder to any free static host and you get a link.

## Easiest: Netlify Drop (about 2 minutes)
1. Unzip `ayah-trace.zip` so you have a folder with `index.html` inside it.
2. Go to https://app.netlify.com/drop
3. Drag the whole folder onto the page.
4. You get a link like `https://something-random.netlify.app`. Create a free account when asked, so the site is not deleted after a day or so.

## Alternative: GitHub Pages (free, permanent address)
1. Create a free account at https://github.com
2. Click **New repository**, name it `ayah-trace`, choose **Public**, click **Create repository**.
3. Click **uploading an existing file**. Drag in `index.html`, `manifest.webmanifest`, `sw.js` and the `icons` folder. Click **Commit changes**.
4. Open **Settings**, then **Pages**. Under Source choose **Deploy from a branch**, branch **main**, folder **/(root)**, then **Save**.
5. Wait one to two minutes. Your app is at `https://YOURNAME.github.io/ayah-trace/`.

## Install it on your phone
- **iPhone:** open the link in **Safari** (not Chrome), tap the Share button, then **Add to Home Screen**.
- **Android:** open the link in Chrome, tap the three-dot menu, then **Install app** (or Add to Home screen).

Open the app once while online. That saves the app and the Arabic font on the phone, and after that it works offline.

## Updating later
1. Replace `index.html` with the new version.
2. In `sw.js`, change `ayah-trace-v1` to `ayah-trace-v2` (then v3, and so on).
3. Upload both files again. Phones update the next time the app opens online.

## Good to know
- Your writing progress is stored on the device in the browser. It does not sync between devices, and clearing the browser's website data erases it.
- The Quran text is from Tanzil.net (CC BY 3.0). Keep the credit line in the app and the license notice inside `index.html`, and do not edit the text itself.
- The page must be served over https. Netlify and GitHub Pages do this automatically. Opening `index.html` straight from your files will not install or work offline.
