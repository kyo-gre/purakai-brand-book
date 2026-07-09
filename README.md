# PuraKai Brand Book

Static, single-page brand book. No build step, no backend, no dependencies to install.

## Structure

```
index.html                  entry point
assets/js/dc-runtime.js     rendering runtime
assets/js/deck-stage.js     page/deck component
assets/js/react*.min.js     React 18.3.1 (vendored, no CDN call at runtime)
assets/img/                 logos, wordmarks, photography
assets/fonts/               Source Serif 4 (woff2 subsets)
```

## Run locally

Open `index.html` over HTTP, not `file://`:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy to Vercel

1. Push this folder to GitHub.
2. Import the repo in Vercel.
3. Framework Preset: **Other**. Leave Build Command and Output Directory blank.
4. Deploy.

Works identically on Netlify, Cloudflare Pages, or GitHub Pages.
