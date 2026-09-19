---
version: alpha
name: Nightpaper
description: Calm dark-navy surfaces, teal accent, serif display type. Gordon's cross-product SaaS theme (first shipped in NomadGuard).
colors:
  primary: "#14B8A6"
  secondary: "#1E3A5F"
  tertiary: "#5EEAD4"
  neutral: "#101E30"
  surface: "#182A40"
  surface-raised: "#16283E"
  border: "#223550"
  ink: "#EDF2F7"
  muted: "#7D8EA3"
  safe: "#22C55E"
  warning: "#F59E0B"
  danger: "#EF4444"
typography:
  display-lg:
    fontFamily: Georgia, 'Noto Serif', serif
    fontSize: 2.375rem
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  display-md:
    fontFamily: Georgia, 'Noto Serif', serif
    fontSize: 1.125rem
    fontWeight: 500
    lineHeight: 1.3
  body-md:
    fontFamily: -apple-system, 'Segoe UI', Roboto, sans-serif
    fontSize: 1rem
    fontWeight: 400
    lineHeight: 1.5
  body-sm:
    fontFamily: -apple-system, 'Segoe UI', Roboto, sans-serif
    fontSize: 0.8125rem
    fontWeight: 400
    lineHeight: 1.5
  label-xs:
    fontFamily: -apple-system, 'Segoe UI', Roboto, sans-serif
    fontSize: 0.6875rem
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "0.02em"
rounded:
  sm: 8px
  md: 12px
  lg: 18px
  full: 999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
components:
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.lg}"
    padding: 16px
  card-title:
    textColor: "{colors.ink}"
    typography: "{typography.display-md}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#06201C"
    rounded: "{rounded.md}"
    padding: 14px
  button-primary-hover:
    backgroundColor: "{colors.tertiary}"
    textColor: "#06201C"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: 14px
  pill-accent:
    backgroundColor: "#22364E"
    textColor: "{colors.tertiary}"
    rounded: "{rounded.full}"
    padding: 6px
  badge-safe:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.safe}"
    rounded: "{rounded.full}"
    padding: 6px
  badge-warning:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.warning}"
    rounded: "{rounded.full}"
    padding: 6px
  badge-danger:
    backgroundColor: "{colors.surface}"
    textColor: "#F87171"
    rounded: "{rounded.full}"
    padding: 6px
  header:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.ink}"
  input:
    backgroundColor: "{colors.neutral}"
    textColor: "{colors.ink}"
    rounded: "{rounded.md}"
    padding: 14px
  text-muted:
    textColor: "{colors.muted}"
  link:
    textColor: "{colors.secondary}"
---

## Overview

Nightpaper is a dark-first identity for utility SaaS products: the calm of
paper-like flat surfaces, transposed to deep navy. Three moves define it —
**flatness** (hairline borders, no shadows, no gradients), **serif display
type** over sans body, and **one accent** (teal) with semantic colors
reserved strictly for state. It should read as a quiet instrument panel,
not a marketing page.

Born as direction C3 of the NomadGuard redesign (2026-08); intended to be
dropped into any future product repo as-is, swapping only the accent if the
product's brand demands it.

## Colors

- **Neutral (#101E30):** App background. Deep navy, never pure black.
- **Surface (#182A40):** Cards, sheets, inputs. One step lighter; separated
  from the background by border, not elevation.
- **Surface-raised (#16283E):** Hero/header zones. Flat — no gradient.
- **Border (#223550):** Hairlines everywhere a shadow would have been.
- **Ink (#EDF2F7) / Muted (#7D8EA3):** Two text tones only. If a third
  seems needed, the hierarchy is wrong.
- **Primary (#14B8A6) / Tertiary (#5EEAD4):** Teal accent and its bright
  variant for text-on-dark-pill use. The only decorative color.
- **Safe / Warning / Danger:** Semantic state only (progress, alerts,
  countdowns). Never used decoratively — that's what keeps them meaningful.

## Typography

Serif display (Georgia / Noto Serif) for identity moments: screen titles,
card titles, and hero numerals (day counts, totals, prices). Everything
else — body, labels, buttons — stays in the platform sans. Numerals in
data displays use tabular figures. Weight discipline: serif at 500,
sans at 400/500; bold is rare and intentional.

## Layout

Generous radii (18px cards, 12px controls), 16px default padding, 4/8/16/24/32
spacing scale. Density over decoration: one idea per card, hierarchy from
scale and spacing, not boxes-within-boxes.

## Elevation & Depth

None. Flatness is the posture: surfaces separate by tone and hairline
border. No drop shadows, no glassmorphism, no gradient fills. Motion
(state transitions, progress sweeps) provides the depth cues instead.

## Components

- **card:** flat surface, hairline border, 18px radius. The workhorse.
- **card-title:** serif, ink — the only serif inside a card.
- **button-primary:** teal fill, near-black text (contrast-safe on teal).
- **pill-accent:** dark pill with bright-teal text for small live values
  ("13 left"), the signature micro-element.

## Do's and Don'ts

- Do keep exactly one accent color per product; swap teal per brand if needed.
- Do give every screen one serif moment — usually the title or the hero number.
- Don't add shadows or gradients; if separation fails, adjust surface tones.
- Don't use safe/warning/danger for anything that isn't state.
- Don't introduce a third text tone or a second decorative color.
