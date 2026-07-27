# Brachial Plexus Tracer

Interactive brachial plexus, upper- and lower-limb nerve palsy tracer. Runs entirely in the browser, works offline, and can be installed on a phone as an app (PWA).

## Files

- `index.html` — the entire app (single file)
- `manifest.json` — app metadata for installation (name, icon, colors)
- `sw.js` — service worker that makes the app work offline
- `icon-192.png`, `icon-512.png`, `icon-512-maskable.png` — launcher icons

## Host it free with GitHub Pages

1. Create a new repository on GitHub (e.g. `plexus-tracer`) and upload all the files in this folder to the repository root.
2. In the repository, go to **Settings → Pages**.
3. Under **Build and deployment**, set Source to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, then click **Save**.
4. After a minute or two your app is live at:
   `https://YOUR-USERNAME.github.io/plexus-tracer/`

## Install on an Android phone

1. Open the GitHub Pages link above in **Chrome** on the phone.
2. Tap the **⋮ menu → Add to Home screen** (Chrome may also show an **Install app** banner).
3. Confirm — the app appears on the home screen with its own icon and opens full-screen like a native app.
4. After the first visit it also works with no internet connection.

## Notes

- The app must be served over HTTPS for installation and offline mode to work — GitHub Pages does this automatically. Opening `index.html` directly from the file system will run the app but won't allow installation.
- To ship an update, just replace the changed files in the repository; phones pick it up on the next visit.
