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

Visual update v6: Removed the eyebrow labels from both game-mode headings. All three pages use the same static dark-blue gradient background; Husky Oddball no longer rotates gameplay backgrounds. Home-page card images remain unchanged.

## v7 updates

- Generator Raid and Husky Oddball mission cards on the home page both rotate their own four image assets every 14 seconds with a 2.4-second fade.
- Each entire card is a keyboard-accessible link to its own game page; the colored action bar remains as the visual affordance.
- Updated `shared-theme.css` to align card spacing, text, colors, buttons, and surfaces with the two gameplay pages.
- Both game-mode pages retain their existing independent local save keys and tracking rules.

## v8 tactical map update

The two maps now use matching subdued L-wall visuals (original orientations preserved) and square-edged tower markers without TWR labels. Husky tower tiles also show their +1 elevation badges.

## King of the Hill (new in v9)
- `husky-king-of-the-hill.html` is an independent five-round tracker using the supplied Husky King of the Hill scenario.
- Round 1 is Hill A; rounds 2–5 randomly choose the remaining hills without replacement.
- Plant/red/blue/clear flag controls. Hill capture scores +5 VP at round end, with +1 VP for each model killed and manual bonus adjustments.
- A distinct localStorage key saves its match separately from Generator Raid and Oddball.
- The four `assets/koth-scene-*.webp` images rotate on the home-page card (14-second interval, 2.4-second crossfade).
- All four pages must be published together in the same GitHub Pages directory, including `shared-theme.css` and `assets/`.


## v11 visual updates
- Restored shared-theme.css and the complete assets folder (missing in prior v10 archive).
- King of the Hill L-walls in B2 and G7; the two provisional orientations can be adjusted later.
- King of the Hill central 1x2 UNSC containers: D4-E4, D5-E5, with a third stacked on E4-E5 (+1 elevation).
- Unified UNSC container styling across all three tactical maps.
- Upload the **contents of this ZIP** to your GitHub Pages publish directory, keeping HTML, CSS and assets at their original relative paths.

### v12 navigation fix
Restored the full navigation layout and button styling to King of the Hill and added shared navigation layout defaults to `shared-theme.css`. Site links and game state keys remain unchanged.

## v14 — King of the Hill map refinements

- The active hill uses one accurately positioned 2×2 outline around the exact four cubes for each zone A–E.
- E4–E5 is depicted as one joined +2-height UNSC container above the two lower 1×2 containers.
- B2 L-wall rotated counterclockwise (bottom-right); G7 L-wall rotated clockwise (top-left).
- G2 and B7 +1 towers use Husky Oddball-style square terrain artwork.
- Generator Raid and Husky Oddball logic and visual maps are unchanged.

## v15 — Homepage label and site icons

The homepage eyebrow reads **HALO FLASHPOINT**. All pages reference the provided favicon, PNG favicon variants, iOS touch icon and web manifest. Keep these icon files and `site.webmanifest` in the same folder as `index.html` when deploying to GitHub Pages. The web manifest uses relative paths so the icons work under a project repository URL.


## Social link preview (v16)

All four HTML pages now include Open Graph and Twitter Card metadata. Upload `share-preview.jpg` to the same folder as `index.html` when publishing via GitHub Pages, and keep `site.webmanifest` and `assets/`. The absolute URLs are set to `https://itsburgertime5000.github.io/Halo-Flashpoint-Game-Companion/`. Sharing previews may be cached by apps.
