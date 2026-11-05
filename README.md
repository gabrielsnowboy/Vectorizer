# Vectorizer

Convert images (PNG, JPG, WebP, GIF, BMP, AVIF) into SVG vector graphics, right in your browser.
Nothing is uploaded — all the tracing happens on your own computer.

## Features

- Drag & drop, click to choose, or paste (Ctrl+V) — several images at once
- Six one-click styles: Logo / flat, Illustration, Photo, Black & white, Posterized, Pixel art
- Fine-tune colors, detail, curve smoothness, blur and working size, with a live preview
- Keeps soft transparency (glows, shadows, smooth cut-out edges) and cleans green-screen fringes
- Optional white-background removal for transparent SVGs
- Side-by-side comparison with the original, with synced zoom (scroll / double-click) and drag-to-pan
- Stacked tracing: color areas overlap instead of touching, so there are no seams between colors
- Download one SVG, download all, or copy the SVG code
- Light and dark mode, works on phones too

## Run it on GitHub Pages

1. Create a new repository on GitHub (for example `vectorizer`), set to **Public**.
2. Click **Add file → Upload files**, drag in `index.html` and `README.md`, then **Commit changes**.
3. Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*,
   pick the **main** branch and the **/ (root)** folder, then **Save**.
4. After a minute or two your app is live at
   `https://<your-username>.github.io/vectorizer/`

You can also just double-click `index.html` to use it offline.

## Updating to a new version

1. In your repo, use **Add file → Upload files**,
   drop in the new `index.html` (it replaces the old one) and **Commit changes**.
2. GitHub Pages can take a few minutes to publish, and browsers cache the old page.
   Press **Ctrl+F5** (Windows) or **Cmd+Shift+R** (Mac) to force a fresh load.
3. Check the version number at the bottom of the page to confirm you're on the latest one.

## Tips

- **Logos and flat art** give the cleanest results. Use *Logo / flat* and lower the color count.
- **Photos** become stylized vector art, not exact copies. Fewer colors and a little blur keep the file size sane.
- **JPGs** have compression noise; a blur of 1–2 px removes the speckles.
- Huge SVGs (several MB) mean too much detail — lower *Colors* or *Detail*, or reduce *Max working size*.

## Credits

Tracing engine: [imagetracerjs](https://github.com/jankovicsandras/imagetracerjs) by András Jankovics,
released into the public domain (The Unlicense). It is bundled inside `index.html`, so the app needs no internet connection.
