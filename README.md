# Adam White — academic website

A single-page GitHub Pages site. Everything lives in `index.md`.

## Publish (one-time setup, ~2 minutes)

1. Create a new GitHub repo named `<your-username>.github.io` (public).
2. Upload the three files: `index.md`, `_config.yml`, and a headshot named `adamHead.jpg` (grab it from https://sites.ualberta.ca/~amw8/adamHead_new.jpg, or delete the `logo:` line in `_config.yml` to skip the photo).
3. On GitHub: Settings → Pages → confirm source is "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Wait a minute; the site appears at `https://<your-username>.github.io`.

## Add a publication (no tools needed)

1. Open `index.md` on github.com and click the pencil (edit) icon.
2. Copy an existing line under the right year, e.g.:

   `- Author One, Adam White. [Paper Title](https://link-to-pdf). *Venue*.`

3. Edit it and click "Commit changes". The site updates itself in ~1 minute.

New year? Add a `### 2026` heading above the 2025 one.

## Change the look

Swap the theme in `_config.yml` for any [supported theme](https://pages.github.com/themes/), e.g. `jekyll-theme-cayman` or `jekyll-theme-slate`. One line, no other changes.
