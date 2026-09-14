# Portfolio 2 — Shivam Soni

UX case-study pages for **Shivam Soni**, built to match Figma
(`Portfolio-Collab`). Plain HTML, CSS and JavaScript — no build tools, no
frameworks.

## Pages

- **`index.html`** — *Sahayya*: redesigning an end-to-end loan origination
  system that cut loan processing from 10 days to 4.
- **`kickfurther.html`** — *Kickfurther*: making an invisible deal-recovery
  process visible to investors, businesses, and the internal team.

## Structure

```
Portfolio-2/
├── index.html                 # Sahayya case study (site entry)
├── kickfurther.html           # Kickfurther case study
├── assets/
│   ├── css/
│   │   ├── styles.css         # shared base: tokens, layout, components, responsive
│   │   └── kickfurther.css    # Kickfurther-only type + components
│   ├── js/
│   │   └── main.js            # scroll-spy, smooth scroll, fade-in, image fallback
│   └── img/
│       ├── sahayya/           # Sahayya graphics
│       └── kickfurther/       # Kickfurther graphics
├── docs/
│   └── figma-assets.md        # source Figma nodes for every exported image
└── README.md
```

## Design system

Shared tokens are CSS custom properties in `:root` (`assets/css/styles.css`):
grey scale (`--grey-40` … `--grey-950`), orange accent (`--orange-400`),
blue, and a `--font-display` token so a page can swap its heading face.

- **Sahayya** — [Geist](https://fonts.google.com/specimen/Geist) +
  [Geist Mono](https://fonts.google.com/specimen/Geist+Mono) (stand-ins for
  the design's licensed *Apercu Pro / Apercu Mono*).
- **Kickfurther** — [Fraunces](https://fonts.google.com/specimen/Fraunces)
  (serif display) + [Ek Mukta](https://fonts.google.com/specimen/Ek+Mukta)
  body + mono labels, via `assets/css/kickfurther.css` overriding the shared
  font tokens.

Both pages share the layout: sticky top nav, sticky left section-nav
sidebar with scroll-spy, and a 768px content column.

## Responsive

Breakpoints at **1080 / 900 / 640 / 400px** — the sidebar collapses to a
horizontal section list, grids and cards stack, and wide diagrams scroll
inside their own container.

## Images

Every graphic is exported from Figma into `assets/img/<project>/`. The map
from filename → source Figma node is in
[`docs/figma-assets.md`](docs/figma-assets.md). Each `<figure class="asset-slot">`
falls back to a labelled placeholder if its image is missing, so the pages
never show broken images.

## Run locally

Open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```
