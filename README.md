# Grey Mist — a Tiger theme

A free, **MIT-licensed** one-page theme for **Tiger** (TigerZF). Self-contained — Bootstrap 5,
Font Awesome, and fonts are all vendored, **no external CDN dependencies**. Adapted from Start
Bootstrap's *Grayscale* (MIT); rebranded and ported to Tiger's theme-module model.

## Install
Drop into the app modules dir (`application/modules/theme-grey-mist/`), then activate it in the
**Module Manager** (Themes) — or set `tiger.theme = grey-mist` + symlink `public/_greymist → assets/`.
Everything is committed (MIT), so a `git clone` is a complete, renderable theme — no fetch step.

## Layout
- `theme.json` — manifest (key `grey-mist`, assetBase `/_greymist`).
- `layouts/scripts/layout.phtml` — chrome (nav + footer) + per-page slots (title/head/scripts).
- `content/index.phtml` — the home body (+ `tiger:page` hint).
- `source/index.html` — the full page (asset pointers repointed to the module's assets).
- `assets/` — css, js, img, and `vendor/` (Bootstrap, Font Awesome, fonts). Committed.
