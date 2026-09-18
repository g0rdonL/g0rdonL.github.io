# gordonlee.xyz

Personal site for Gordon Lee — AI automation consulting for Hong Kong SMBs. Static, no build step, served via GitHub Pages.

- `index.html` — the whole site: content, styles and the theme toggle script
- `og-image.png` — social preview image
- `robots.txt`, `sitemap.xml` — SEO
- `CNAME` — custom domain (gordonlee.xyz)

## Design

- Type: Fraunces (display serif), Schibsted Grotesk (body), DM Mono (labels and prices); Noto Serif SC / Noto Sans SC for Chinese
- Colour: warm ivory ground, near-black ink, one brick accent; light and dark themes follow the system and can be toggled in the header
- Bilingual: every English line is followed by its Simplified Chinese counterpart in a `.zh` span
- Layout breakpoints use container queries on `.page`, so the same CSS renders correctly inside fixed-width mockups

## Local preview
```
python3 -m http.server 8000
```
