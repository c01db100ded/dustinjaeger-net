# dustinjaeger.net — IT Portfolio

A living portfolio site redesigned with **taste-skill** principles. Gets better every night.

## What This Is
- **Domain:** [dustinjaeger.net](https://dustinjaeger.net)
- **Hosting:** GitHub Pages (free, auto-deploys on push)
- **Source:** This repo → GitHub Pages
- **Design:** Dark-first, teal accent (#22d3aa), semantic color tokens

## Tech Stack
- **HTML/CSS/JS** — Zero frameworks, single-file `index.html` + `links-page.html`
- **Variable fonts:** Space Grotesk (display) + JetBrains Mono (code/data)
- **CSS Grid** for macro layout, CSS custom properties for theming
- **Dark mode first** — respects `prefers-color-scheme`, light mode available
- **Accessibility:** `prefers-reduced-motion` disables all animations
- **Performance:** Incremental scroll reveal via IntersectionObserver

## File Structure
```
dustinjaeger-net/
├── index.html          # Main portfolio (single-page)
├── links-page.html     # Curated links & resources (60KB+)
├── CHANGELOG.md        # Nightly changes log
├── CNAME               # Custom domain: dustinjaeger.net
├── README.md           # This file
├── assets/             # Images, icons
├── scripts/            # Build scripts (if any)
└── .github/workflows/  # CI/CD
```

## Deployment
1. Push to `main` → GitHub Actions deploys to GitHub Pages
2. Custom domain `dustinjaeger.net` via `CNAME` file
3. Changes live within ~1 minute of push

## Key Features
- **Asymmetric skills grid** — featured card spans 2 columns, no "three equal cards" AI slop
- **Semantic color tokens** — single accent hue, dark mode first
- **Savings badges** — distinct green for quantified achievements
- **Links page** — 10+ sections, rolling 30-day "New Links" list, pentesting/gadget firmware, AI, emulation, Linux
- **Zero frameworks** — no React, no build step, pure HTML/CSS/JS

## Changelog
See [CHANGELOG.md](CHANGELOG.md) for nightly updates.

## Local Development
```bash
# Just open index.html in a browser
# Or serve locally:
npx serve .
# or
python -m http.server 8000
```