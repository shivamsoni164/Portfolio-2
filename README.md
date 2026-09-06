# Portfolio 2 — Sahayya case study

A single-page UX case study for **Shivam Soni**, built to match the Figma
design (`Portfolio-Collab` → `Sahayya Page`). Plain HTML, CSS and
JavaScript — no build tools, no frameworks.

> **Sahayya** — how a redesign of an end-to-end loan origination system cut
> loan processing time from 10 days to 4, for India's self-employed borrowers.

## Structure

```
Portfolio-2/
├── index.html      # Page markup (nav, sidebar, all sections, footer)
├── styles.css      # Design tokens + all styles + responsive breakpoints
├── main.js         # Scroll-spy, smooth scroll, fade-in, image fallback
├── images/         # Exported Figma graphics (see images/README.md)
└── README.md
```

## Design system

Tokens live as CSS custom properties in `:root` (`styles.css`):

- **Colour** — grey scale (`--grey-40` … `--grey-950`), orange accent
  (`--orange-400 #ff5630`), blue (`--blue #3b41e3`), warm persona card.
- **Type** — [Geist](https://fonts.google.com/specimen/Geist) for
  headings/body and [Geist Mono](https://fonts.google.com/specimen/Geist+Mono)
  for labels (loaded from Google Fonts). These stand in for the design's
  licensed *Apercu Pro / Apercu Mono*; Geist is also used in the original
  design, so the substitution stays close.
- **Layout** — sticky top nav, sticky left section-nav sidebar, and a
  768px content column.

## Sections

Overview (hero) → Introduction → The Customer → The Research → The Problems
→ Solution 01 → Solution 02 → Solution 03 → Footer.

## Responsive

- **≤ 1080px** — tighter gutters and sidebar.
- **≤ 900px** — sidebar collapses to a horizontal section list above the
  content; persona card stacks.
- **≤ 640px** — meta grid drops to 2 columns, nav condenses, footer stacks.
- **≤ 400px** — meta grid single column.

## Images

Four raster graphics need a manual export from Figma — see
[`images/README.md`](images/README.md). The page renders labelled
placeholders until they're added, so it works as-is.

## Run locally

Just open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```
