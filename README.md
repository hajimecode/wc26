# WC26 — World Cup 2026 Interactive Hub

The Nike-editorial-style interactive companion to the 2026 FIFA World Cup.
INK base · LIME accent · Krona One typography · 48 nations · 104 matches.

## Stack
- Single-file React app via CDN (Babel-transpiled at runtime)
- Tailwind CSS via CDN
- Static deployment (no backend)

## Sections
- **Home** — hero, fixtures, briefing, navigation
- **News** — articles, filters, full editorial layout
- **Schedule** — 104 matches, day list, groups, bracket
- **Predict** — 90-minute Poisson simulator with intangible factors
- **Teams** — 48 nations × full squad analytics + tactical board
- **Analysis** — drag-and-drop tactical board (two formations side-by-side)

## Local dev
Open `index.html` directly in a browser, or serve with any static server:

```bash
npx serve .
# or
python3 -m http.server 8080
```

## Deployment

Deployed via Vercel. The project root is this folder.

Custom domain: **wc26.tech**

### vercel.json highlights
- SPA fallback: all routes → `/index.html` (so client-side hash routing works after refresh)
- Long-term caching for `/images/*`
- Short cache for `*.json` (news content)

## License
Independent fan project — not affiliated with FIFA.
© 2026 WC26
