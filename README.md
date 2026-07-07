# Adam White — academic website

A single-page GitHub Pages site. Everything lives in `index.md`.

## Publish (one-time setup, ~2 minutes)

1. Create a new GitHub repo named `<your-username>.github.io` (public).
2. Upload everything in this folder, keeping the structure: `index.md`, `_config.yml`, `adamHead_new.jpg`, and the `assets/css/style.scss` file (this styles the profile card at the top — without it the header will look plain).
3. On GitHub: Settings → Pages → confirm source is "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Wait a minute; the site appears at `https://<your-username>.github.io`.

## Add a publication (no tools needed)

1. Open `index.md` on github.com and click the pencil (edit) icon.
2. Copy an existing line at the top of the right section (Journal Papers, Conference Papers, etc.), e.g.:

   `- Author One, Adam White (2026). [Paper Title](https://link-to-pdf). *Venue*.`

3. Edit it and click "Commit changes". The site updates itself in ~1 minute.

## Change the look

Swap the theme in `_config.yml` for any [supported theme](https://pages.github.com/themes/), e.g. `jekyll-theme-cayman` or `jekyll-theme-slate`. One line, no other changes.
