# Longevity Diet — Landing Page

A single-page, self-contained landing page for the Healthy Kitchen "Longevity Diet" meal plan (Dubai). Built as one static `index.html` with React + Babel loaded from CDN — no build step, no dependencies to install.

## Structure

```
index.html        The complete landing page (markup, styles, and React/JSX inline)
assets/           Images referenced by the page (dishes, hero, logos)
```

## Run locally

Because the page fetches images from `assets/`, open it through a local web server rather than the `file://` protocol:

```bash
# Python 3
python3 -m http.server 8000
# then open http://localhost:8000
```

Any static server works (`npx serve`, VS Code Live Server, etc.).

## Deploy

It's a static site — drop the folder onto any static host:

- **GitHub Pages** — push this folder to a repo, enable Pages on the branch root.
- **Netlify / Vercel / Cloudflare Pages** — set the publish directory to this folder, no build command.

## Notes

- React, ReactDOM, and Babel are loaded from `unpkg.com` at runtime; an internet connection is required on first load.
- Fonts are pulled from Google Fonts.
