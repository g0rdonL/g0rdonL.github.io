# gordonlee.xyz

Personal site for Gordon Lee — AI automation consulting for Hong Kong SMBs. Static, no build step, served via GitHub Pages.

- `index.html` — the whole site: content, styles and the theme toggle script
- `og-image.png` — social preview image
- `robots.txt`, `sitemap.xml` — SEO
- `CNAME` — custom domain (gordonlee.xyz)

## Design

The site uses the [Nightpaper](https://github.com/g0rdonL/nightpaper) theme; `DESIGN.md` is a copy of its spec (tokens in the front matter, rationale in prose). Read it before changing any UI.

- Colour: navy neutral / surface / surface-raised, hairline borders, one teal accent; ink and muted are the only two text tones
- Type: Georgia display for titles and prices, platform sans for everything else; no web fonts
- Flat: no shadows, gradients or glass; 18px cards, 12px controls, pill for small live values
- Bilingual: every English line is followed by its Simplified Chinese counterpart in a `.zh` span
- Layout breakpoints use container queries on `.page`, so the same CSS renders correctly inside fixed-width mockups

## Local preview
```
python3 -m http.server 8000
```
