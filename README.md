# Yash Todkari — Product Portfolio

A single-page, static portfolio site for Yash Todkari (Product Manager · Product Owner · Business Analyst).

No backend, no build step, no dependencies to install — plain HTML, CSS, and vanilla JavaScript.

## What's inside

```
.
├── index.html          # the entire site (markup + styles + scripts)
└── assets/
    ├── favicon.svg
    ├── profile-photo.jpg
    ├── resume.pdf
    ├── investment-guardian.pdf
    ├── notion-product-teardown.pdf
    └── genai-product-discovery.pdf
```

## Running it locally

Just open `index.html` in a browser — no server required. If your browser blocks local PDF embeds, run a tiny local server instead:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

This is a static site, so it works as-is on any static host:

- **GitHub Pages** — push this repo, then enable Pages in Settings → Pages → Deploy from branch (`main`, root).
- **Netlify / Vercel / Cloudflare Pages** — drag-and-drop the folder or connect the repo; no build command needed (or leave the build command empty / set output directory to `/`).

## Updating content

- Swap any file in `assets/` (keeping the same filename) to update the resume, case-study PDFs, or photo.
- Text content lives directly in `index.html` — search for the relevant section heading (`<section id="...">`) to edit copy.
- Colors, type, and spacing are defined as CSS custom properties at the top of the `<style>` block (`:root` for light mode, `[data-theme="dark"]` for dark mode).

## Notes

- Dark/light mode defaults to system preference, with a manual toggle in the nav.
- Fully respects `prefers-reduced-motion`.
- Investment Guardian and the Notion Product Teardown are both clearly labeled as independent concept work, not official or shipped products.
