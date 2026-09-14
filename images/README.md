# Images

Graphics exported from the Figma file (`Portfolio-Collab` → `Sahayya Page`,
node `13:1399`) and used across the case study.

| File                     | Section                                   | Figma node |
|--------------------------|-------------------------------------------|------------|
| `persona-suresh.png`     | "Meet Suresh" persona card                | `56:104`   |
| `research-journey.png`   | Typical-journey service blueprint         | `56:151`   |
| `dependency-matrix.png`  | 13 × 13 stage dependency matrix (heatmap) | `62:1421`  |
| `rules-table.png`        | The 91 reopen-rules table                 | `62:2566`  |
| `asset-checks.png`       | Asset / Document checks UI                 | `63:4622`  |
| `sql-error.png`          | SQL-exception error dialog                | `65:4628`  |

To replace any of these, export the node again (PNG, 2x) and overwrite the
file with the same name — the page references them by these filenames.

> The page hero (top of `index.html`) is a plain tinted block, matching the
> placeholder in the source design. To use a real image there, drop
> `hero.png` into this folder and restore the `<img>` in the hero `<figure>`.

---

## Kickfurther case study (`kickfurther.html`)

Same as above — export each node from Figma (`Portfolio-Collab` → `KF Page`,
node `141:1031`) as **PNG, 2x** and save it here with the exact filename.
Until then each slot shows a labelled placeholder.

| Filename                | What it is                                  | Figma node | Approx. size |
|-------------------------|---------------------------------------------|------------|--------------|
| `kf-hero.png`           | "Fund your inventory" hero graphic          | `201:1790` | 768 × 513    |
| `kf-marketplace.png`    | How the marketplace works (diagram)         | `172:1329` | 768 × 337    |
| `kf-happy-path.png`     | The happy-path process map                  | `182:1632` | 768 × 420    |
| `kf-blueprint-1.png`    | Service blueprint — frame 1                  | `201:1774` | 962 × 398    |
| `kf-blueprint-2.png`    | Service blueprint — frame 2                  | `201:1776` | 962 × 389    |
| `kf-blueprint-3.png`    | Service blueprint — frame 3                  | `201:1778` | 962 × 382    |
| `kf-investor.png`       | Investor deal-detail view (UI)              | `188:1655` | 768 × 253    |
| `kf-business.png`       | Business dashboard (UI)                     | `188:1660` | 768 × 456    |
| `kf-team-flow.png`      | Team workflow / service diagram             | `188:1662` | 840 × 193    |

The promise cards, the compliance/alert widget, and the 50% / 40% stat tiles
are recreated in HTML/CSS (responsive), so they need no export.
