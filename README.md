# Recipe Box

A tabbed recipe box of index cards that you can install to your phone's home screen. It works offline.

## Files

| File | Purpose |
|---|---|
| `index.html` | The whole app (HTML, CSS, JS) |
| `manifest.json` | Name, colors and icons for the home screen install |
| `sw.js` | Service worker that caches the app so it opens offline |
| `icons/` | App icons (Android, iOS, favicon) |

## Put it on GitHub Pages

1. Create a new repo (for example `recipe-box`) and upload all of these files, keeping the `icons` folder.
2. Go to **Settings → Pages**, set Source to **Deploy from a branch**, then pick `main` / root.
3. After a minute it's live at `https://<username>.github.io/recipe-box/`.

## Add to home screen

- **iPhone (Safari):** Share → Add to Home Screen
- **Android (Chrome):** ⋮ menu → Add to Home screen / Install app

## Updating

After you change `index.html`, bump `VERSION` in `sw.js` (for example `recipe-box-v2`) so installed copies pick up the new version.

## Data

Recipes are saved in the browser's local storage on each device. Use **Backup / restore** to copy them out or move them to another device.
