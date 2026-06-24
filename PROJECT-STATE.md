# PROJECT-STATE.md — Vinh Portfolio

**Status:** Ready for deployment
**Last updated:** 2026-06-24

## Current Phase

Portfolio page built and rendering correctly. Awaiting GitHub Pages deployment.

## Locked Decisions

- **Format:** Single self-contained `index.html` (no Jekyll, no framework)
- **Theme:** Minimalist Editorial / Magazine style (White `#ffffff` bg, Red `#c0392b` accent)
- **Fonts:** Instrument Serif (headings) + Stack Sans Text / Inter (body)
- **Sections:** About (Profile & Chronological Experience) → Showreel (Selected Work) → Brands (Collaborators)
- **Deployment target:** GitHub Pages via `<username>.github.io` repo

## Data Sources Used

| Source | Content | Method |
|--------|---------|--------|
| LinkedIn | Experience, title, headline, connections | User screenshots (HTTP 999 block) |
| PDF Bio | Director intro, brands, portfolio links | `read` text extraction |
| Notion AI Creator Hub | Tech stack, services, workshops, teaching | `mcp__notion_fetch` |
| Notion VINHLAM Agent | AI persona, products, methods, brand voice | `mcp__notion_fetch` |
| Reference site | Layout structure (linhkid.github.io) | `browser` HTML extraction |

## Open Design Status

- Daemon was not reachable during build (port 7456 connection refused)
- MCP tools are discoverable but daemon must be running
- Page built directly with hand-crafted HTML/CSS
- Can re-run through OD design pipeline later if daemon comes up

## Next Steps

- [ ] Deploy to GitHub Pages
- [ ] Add profile photo (replace emoji placeholder in `.avatar`)
- [ ] Add OG image for social shares (`assets/og-image.jpg`, 1200x630)
- [ ] Optionally run through Open Design for polish pass
- [ ] Add Google Analytics or GoatCounter (like reference site)
- [ ] Consider adding a Projects/Portfolio gallery section with video embeds
