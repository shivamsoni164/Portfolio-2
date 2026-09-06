# Images to export from Figma

These four graphics are raster/vector artwork from the Figma file that
can't be recreated faithfully in code. Export each one from the source
Figma file and drop it in this folder using the **exact filename** below —
the page picks them up automatically. Until then the page shows a labelled
placeholder in each slot (nothing breaks).

**Source file:** `Portfolio-Collab` — page frame `Sahayya Page` (node `13:1399`)

| Filename                     | What it is                                   | Figma node | Approx. size |
|------------------------------|----------------------------------------------|------------|--------------|
| `hero.png`                   | Project hero image (top of page)             | `13:1429`  | 766 × 512    |
| `suresh.jpg`                 | Persona photo — Suresh, the restaurant owner | `56:104`   | portrait     |
| `research-journey.png`       | "Typical Journey" service blueprint diagram  | `56:151`   | 761 × 325    |
| `dependency-matrix.png`      | 13 × 13 stage dependency matrix (heatmap)    | `62:1421`  | 768 × 630    |
| `rules-table.png`            | The 91 reopen-rules table (status vs. stage) | `62:2566`  | 768 × 158    |

## How to export

1. Open the Figma file and select the node (right-click → *Copy/Paste as* is
   not needed — just select the layer by its node id / name).
2. In the right-hand **Export** panel, add an export setting: **PNG, 2x**
   (use **JPG** for `suresh.jpg`).
3. Export and save into this `images/` folder with the filename above.

> Note: these were originally going to be pulled automatically through the
> Figma MCP, but this environment's network policy blocks downloads from
> `figma.com`, so they need a manual export. Everything else on the page —
> layout, type, colours, the persona card, the Asset-Checks table and the
> SQL-error dialog — is built in HTML/CSS and is fully responsive.
