# Halo: Flashpoint Game Companion

Multi-page static website with two independent game-mode trackers.

## Files
- `index.html` — companion home page / game mode selection
- `generator-raid.html` — Generator Raid tracker
- `husky-oddball.html` — Husky Oddball: Reloaded tracker
- `assets/halo-scene-1.webp` … `halo-scene-4.webp` — optimized local background images

## Publishing with GitHub Pages
Upload **all files and the `assets` folder** to the root of the GitHub Pages publishing branch. Ensure `index.html` is at the root. In repository Settings → Pages, confirm the source branch and root folder. After deploying, open your GitHub Pages URL.

The two trackers use separate localStorage keys, so progress is independent. Existing Generator Raid and Husky Oddball local save data remains accessible when running from the **same origin** as before, as long as it used the same localStorage keys. Changing the hosting address changes the storage origin.

No build step or external dependency is required. Open `index.html` locally or use any static web server.
