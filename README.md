# Vinh Lam — Personal Portfolio

A single-page portfolio for [Vinh Lam](https://vinhlam.com) — Film Director, Creative Technologist, and Visual Artist.

## Live Site

→ **[vinhlamphuoc.github.io](https://vinhlamphuoc.github.io/)** (once deployed)

## Quick Start

```bash
# Preview locally
open index.html

# Or serve with any static server
npx serve .
python3 -m http.server 8000
```

## Deploy to GitHub Pages

```bash
# 1. Create a repo named <your-username>.github.io on GitHub

# 2. Initialize and push
cd ~/Desktop/vinh-portfolio
git init
git add .
git commit -m "Initial portfolio"
git branch -M main
git remote add origin git@github.com:<your-username>/<your-username>.github.io.git
git push -u origin main

# 3. GitHub Pages auto-serves from main branch root
#    Settings → Pages → Source: Deploy from branch (main / root)
```

## Project Structure

```
vinh-portfolio/
├── index.html          # Self-contained portfolio (all CSS/JS inline)
├── README.md           # This file
├── PROJECT-STATE.md    # Current state and locked decisions
└── assets/             # (optional) Add profile photo, OG image later
    └── og-image.jpg    # Social share preview (1200x630 recommended)
```

## Customization

Everything is in `index.html` — no build step, no dependencies (except Google Fonts CDN).

### Change accent color
Find `--accent: #c8ff00;` in the `:root` CSS block. Swap to any hex color. The `--accent-dim` and `--gradient` variables derive from it.

### Add profile photo
Replace the `.avatar` div's emoji placeholder with an `<img>` tag:
```html
<div class="avatar"><img src="assets/profile.jpg" alt="Vinh Lam" style="width:100%;height:100%;object-fit:cover;"></div>
```

### Add/remove sections
Each `<section>` is independent. Copy, reorder, or delete freely. Update nav links to match.

### Update content
All text is inline HTML — edit directly. Key sections:
- **Hero**: `.hero-text h1` and `.hero-text p`
- **About**: `.about-text` paragraphs
- **Experience**: `.timeline-item` blocks
- **Services**: `.service-card` blocks
- **Brands**: `.brand-pill` spans
- **Toolkit**: `.tool-card` divs
- **Contact**: `.contact-links` anchors

## Sources

Built from:
- LinkedIn profile ([linkedin.com/in/vinhwalter](https://linkedin.com/in/vinhwalter))
- Director's Bio PDF (2026)
- Notion AI Creator Hub & VINHLAM personal AI Agent pages
- Reference: [linhkid.github.io](https://linhkid.github.io/) layout structure

## Tech

- Pure HTML + CSS + vanilla JS (IntersectionObserver)
- Google Fonts: Space Grotesk + Inter
- No frameworks, no build tools, no npm
- ~27KB single file
