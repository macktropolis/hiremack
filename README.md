# hiremack.com

Personal CV and portfolio site for Mack Richardson — FileMaker & Web Developer.

**Live site:** [hiremack.com](https://hiremack.com)

---

## Stack

Plain HTML, CSS, and a small amount of vanilla JavaScript. No build step, no dependencies, no frameworks. Hosted on Netlify with continuous deployment from this repository.

- **Fonts:** [DM Sans](https://fonts.google.com/specimen/DM+Sans), [DM Serif Display](https://fonts.google.com/specimen/DM+Serif+Display), [DM Mono](https://fonts.google.com/specimen/DM+Mono) via Google Fonts
- **Hosting:** Netlify
- **Domain:** Managed via DNS pointing to Netlify

---

## Repository Structure

```
├── index.html          # Single-page CV site
├── styles.css          # All styles
├── sitemap.xml         # XML sitemap for search engines
├── robots.txt          # Crawler directives
├── _redirects          # Netlify redirect rules
├── assets/
│   ├── images/         # Photos, logos, certification badges, project screenshots
│   └── downloads/
│       └── mack-richardson-cv.pdf
└── README.md
```

---

## Local Development

No build process required. Open `index.html` directly in a browser, or serve it with any static file server:

```bash
# Python
python -m http.server 8000

# Node (npx)
npx serve .
```

---

## Deployment

Netlify watches the `main` branch. Pushing to `main` triggers an automatic deploy. There is no build command — Netlify serves the repository root directly.

**Netlify build settings:**
- Build command: *(none)*
- Publish directory: `/`

---

## Updating Content

| Task | File |
|---|---|
| Update work experience, projects, or bio | `index.html` |
| Change colors, fonts, or layout | `styles.css` |
| Replace CV PDF | `assets/downloads/mack-richardson-cv.pdf` |
| Update sitemap date after content changes | `sitemap.xml` → `<lastmod>` |

---

## License

&copy; Mack Richardson. All rights reserved. This repository is public for transparency — the code and content are not licensed for reuse.
