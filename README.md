# PixelPlay — Neon Cyberpunk Browser Arcade

A responsive static gaming portal inspired by the *type* of experience offered by large browser-game sites, with an original neon-cyberpunk visual identity. Built with HTML, CSS, and vanilla JavaScript for GitHub Pages.

## Included features
- Responsive desktop, tablet, and mobile layout
- Top navigation, search, category filters, game cards, and related games
- Dedicated game pages (`play.html?game=...`)
- Fullscreen game-stage button where supported by the browser
- Save/remove favorites with browser local storage
- Eight playable demos: Neon Drift, Cyber Snake, Neon Dodger, Memory Grid, Reaction Rush, Coin Frenzy, Orbit Lab 3D, and Sky Hop
- Keyboard controls and touch buttons for supported games
- No build step, package manager, or server required

## Run locally
1. Extract the ZIP.
2. Open `index.html` in a modern browser.
3. Click any game card. The 3D Orbit Lab demo loads Three.js from a CDN, so it requires an internet connection. The other demos run locally.

For best results, test through a local static server or GitHub Pages, especially for the 3D demo.

## Publish free with GitHub Pages
1. Sign in to GitHub and create a new repository, for example `pixelplay`.
2. Upload **the contents of this folder** (not the ZIP file itself) to the repository root. `index.html` must be at the root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select branch `main` and folder `/(root)`, then press **Save**.
6. Wait for the published URL to appear on the Pages settings screen. It usually looks like `https://YOUR-USERNAME.github.io/pixelplay/`.
7. Open that URL and test search, categories, each game, mobile layout, and fullscreen.

## How to add a game card
Open `js/catalog.js` and add an object to `PIXELPLAY_GAMES`. The `kind` value must match a game implementation in `js/player.js` to make the card playable. The card metadata is rendered automatically on the homepage and the individual game page.

## Important limitations
- These are original lightweight playable demos, not full commercial games or replicas of third-party titles.
- GitHub Pages is static hosting. Accounts, cross-device save sync, online multiplayer, shared leaderboards, and server-side APIs require a separate backend.
- Favorites are stored only in the visitor's current browser.
- Orbit Lab uses the Three.js CDN and Google Fonts uses Google Fonts. If those external services are blocked, the portal still loads, but those assets may not.
- Fullscreen depends on browser support and user gesture/security restrictions.
- Before public launch, check every game on your target devices and consider adding original art, audio, accessibility testing, privacy information, and terms appropriate to your project.
