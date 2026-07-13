# Grey Mist

A **free, MIT-licensed one-page theme** for the [Tiger](https://github.com/WebTigers/TigerCore)
platform — self-contained, zero external dependencies, and built to be *read and edited*.

Grey Mist is Tiger's reference theme: proof that a theme installs, activates, and renders through
the Module Manager with nothing but a config flip and an asset symlink. It's also a clean starting
point for your own site — fork it, restyle it, ship it.

![Grey Mist](https://raw.githubusercontent.com/WebTigers/theme-grey-mist/v0.1.0-beta/assets/img/bg-masthead.jpg)

## What you get

- **One-page layout** — masthead, about, projects, signup, and contact sections, ready to rework.
- **Bootstrap 5.3.8**, shipped as **readable, un-minified CSS & JS**. No build step, no compiled
  blobs — every style is yours to open and change. That's the point: themes are for devs and CMS
  authors, so nothing is obfuscated.
- **Zero phone-home.** Fonts, Font Awesome, and all assets are vendored locally — no CDN, no
  third-party form host, no tracking. Interactive pieces (like the newsletter form) are static
  markup you wire up *inside Tiger*.
- **Theme-as-a-module.** A single `theme.json` manifest (`key: grey-mist`, `assetBase: /_greymist`)
  is all the Module Manager needs to discover, preview, and activate it.
- **Editable everything** — `layouts/` for the chrome, `content/` for the page bodies, `source/`
  for the pristine reference page, `assets/` for the CSS/JS/fonts/images.

## Install & activate

1. In Tiger admin, go to **Modules → Add New → Browse the directory** and find **Grey Mist**.
2. **Install**, then **Activate**. Tiger writes `tiger.theme = grey-mist` and symlinks the theme's
   assets to `/_greymist` — no deploy, effective on the next request.
3. Your public site now renders in Grey Mist. The admin/back office stays on the platform theme
   (a public theme never touches the admin).

To preview before committing, use the Module Manager's **Preview** (an admin-only cookie) so only
you see it while the live site is unchanged.

## Make it yours

- Restyle by editing `assets/css/grey-mist.css` (the accent palette lives at the top as `--bs-*`
  overrides) — or drop in a Bootstrap skin.
- Edit the page bodies in `content/*.phtml`; each carries a small `tiger:page` hint for its title
  and layout.
- A CMS page with the same slug always overrides the theme's file — so you can override any page
  from the admin without touching the theme.

## License & credits

MIT — use it for anything, personal or commercial. Adapted from
[Start Bootstrap – Grayscale](https://startbootstrap.com/theme/grayscale) (also MIT), rebranded and
re-homed for Tiger by [WebTigers](https://webtigers.com). See
[LICENSE](https://github.com/WebTigers/theme-grey-mist/blob/main/LICENSE).
