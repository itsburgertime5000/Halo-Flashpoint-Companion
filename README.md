# Halo: Flashpoint Game Companion

Static GitHub Pages website with three pages:

- `index.html` — Mission selection
- `generator-raid.html` — Generator Raid tracker, static dark gradient background
- `husky-oddball.html` — Husky Oddball: Reloaded tracker, rotating Oddball screenshots
- `shared-theme.css` — Unified colors, typography, buttons, spacing, cards and navigation
- `assets/` — Image assets for the home page and other visuals

## Deploy
Upload **all files and the assets folder** from this ZIP into the branch/folder used by GitHub Pages. Keep the HTML files and shared stylesheet in the same directory. Opening `index.html` launches the mission-selection page.

Both game modes save their state independently to browser localStorage, using their existing storage keys. The website does not require a backend.

Updating the site does not intentionally clear either game's saved data.
