# HoR AMR Fuji 2026 Driver Debrief — Safari site

This folder is ready to upload as a static website. Drivers only need the HTTPS link in Safari; no TestFlight or app installation is required.

## GitHub Pages
1. Create a new GitHub repository (for example `hor-fuji-debrief`).
2. Upload **all files in this folder** to the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select `main` and `/ (root)`, then Save.
6. GitHub will provide an HTTPS link. Open that link in Safari.

## Cloudflare Pages
1. Create a Pages project.
2. Upload this folder / ZIP using Direct Upload, or connect the GitHub repository.
3. No build command is required; the output directory is the site root.
4. Use the HTTPS link Cloudflare provides.

## iPhone use
Open the HTTPS link in Safari. Optionally use **Share → Add to Home Screen**. The included manifest, Apple touch icon and service worker make it behave more like an app and cache the static page for offline reopening after the first successful load.

## Email button
The current **Send to Engineers** button prepares an email addressed to `mgrigalauskas@prodrive.com` using the device's mail app. It does not send silently.

## Track map
The embedded official WEC / Al Kamel Fuji circuit map is loaded from the Al Kamel website, so that map itself needs an internet connection unless it is later bundled locally.
