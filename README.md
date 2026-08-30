# Ski Cards — 29 Dec 2026 → 6 Jan 2027

A phone-first flashcard deck for choosing a ski destination. 34 options, ranked by
**experience per dollar** rather than by price.

Static site. One self-contained `index.html`, no build step, no dependencies, no backend.

## What's here

| File | Purpose |
|---|---|
| `index.html` | The whole app — data, styles and logic inlined |
| `manifest.webmanifest` | Lets it install to a phone home screen |
| `icon-192.png` `icon-512.png` `apple-touch-icon.png` | App icons |
| `_headers` | `noindex` + security headers (works on Cloudflare Pages *and* Netlify) |
| `robots.txt` | Keeps it out of search engines |

## Deploying to Cloudflare Pages

1. Push this repo to GitHub.
2. Cloudflare dashboard → **Workers & Pages** → **Create** → **Pages** → **Connect to Git**.
3. Authorise the Cloudflare Pages GitHub App and pick this repo.
4. Build settings — leave everything empty:
   - Framework preset: **None**
   - Build command: *(blank)*
   - Build output directory: `/`
5. **Save and Deploy.**

Every push to `main` redeploys automatically from then on. That is the auto part.

## Source of the numbers

Merged from two planning workbooks and re-verified against official resort tariffs on
30 Aug 2026. Hakuba Valley and Niseko United 2026/27 lift prices confirmed exact.
Shiga Kogen and Tatry Super Ski corrected. **No flight fare or accommodation figure
here is a verified quote** — those sites block automated price reads. Price them yourself.

Full model, reconciliation and verification log live in the companion spreadsheet.
