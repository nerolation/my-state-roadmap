# Ethereum State Roadmap

A strawman, lane-by-lane roadmap of Ethereum **state** proposals (EIPs), inspired by
[strawmap.org](https://strawmap.org). Forks run left → right; lanes group proposals by the
lever they pull over a state object's lifecycle. Placements are indicative, not a schedule.

## Files

- **`state-roadmap.html`** — the roadmap viewer (served at the site root via `index.html`).
- **`state-roadmap-editor.html`** — a drag-and-drop editor to rearrange tiles, then
  **Export → Download `roadmap-data.js`** to commit the new layout.
- **`roadmap-data.js`** — the single source of truth (forks, lanes, tiles). Both pages read it.

Pure static site — no build step. Styling via the Tailwind CSS v4 browser CDN; drag-and-drop
via SortableJS (both loaded from a CDN, so viewing needs network access).
