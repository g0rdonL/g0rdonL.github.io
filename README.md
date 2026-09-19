# gordonlee.xyz

Personal site for Gordon Lee — AI automation consulting for Hong Kong SMBs. Static, no build step, served via GitHub Pages.

- `index.html` — the whole site: content and styles
- `DESIGN.md` — Nightpaper theme spec (copied from the theme repo)
- `og-image.png` — social preview image
- `robots.txt`, `sitemap.xml` — SEO
- `CNAME` — custom domain (gordonlee.xyz)

## Design

The site uses the [Nightpaper](https://github.com/g0rdonL/nightpaper) theme; `DESIGN.md` is a copy of its spec and is the source of truth for tokens. Read it before touching the UI.

- Colour: dark navy surfaces (`#101E30` / `#182A40`), hairline borders, one teal accent (`#14B8A6`); dark only, no theme toggle
- Type: Georgia / Noto Serif for titles and hero numbers, platform sans for everything else; Noto Serif SC / Noto Sans SC for Chinese
- Flat: no shadows, gradients or glass; 18px cards, 12px controls
- Bilingual: every English line is followed by its Simplified Chinese counterpart in a `.zh` span
- Layout breakpoints use container queries on `.page`, so the same CSS renders correctly inside fixed-width mockups

## Local preview
```
python3 -m http.server 8000
```
