# README artwork

Three lossless PNG compositions used by the README. Styling is baked into the images; GitHub rendering needs no custom CSS, scripts or installed fonts. The opening uses the existing `../brand/gentle-shell-banner.gif`, not a new static hero.

| Asset | Size | Source and composition |
| --- | --- | --- |
| `changes.png` | 1600 × 1120 | Continuous crop `(10, 0, 1260, 595)` of `../features/changes-view.png`: worktree list beside the real diff. |
| `agents.png` | 1600 × 1120 | Continuous crop `(0, 0, 1000, 477)` of `../features/agents-view.png`: session list, completed-worker status, model and handoff. Enlarged to a comparable text scale to Changes; long handoff lines are clipped, with the full source linked in the README. |
| `control.png` | 1600 × 1120 | An explanatory diagram, not product UI, adapted from `../diagrams/permission-modes.svg`. |

Crop rectangles use Pillow's left/top/right/bottom coordinates. The Changes and Agents panels contain no fabricated output, recoloring, overlays on evidence, rearranged terminal fragments or recreated UI. Crops may clip long lines; the full source screenshots remain available in README disclosures. These illustrative sessions are not claimed output of a new installation walkthrough.

## Visual identity

The palette and geometric terminal motif come from `../brand/gentle-pi-banner.svg`: dark plum, luminous `#f095c8`, muted `#d7a0b8` and warm white. Andale Mono typography was rasterized during production. Numbers, rules, contours, corner brackets, shadows and gradients sit outside screenshot evidence pixels.

The three files total 1,088,163 bytes. They were composed with Python Pillow during local design iteration; the preview and production scripts are not shipped in this directory. Viewing the finished PNGs needs neither Pillow nor the original font.

## Evidence and boundaries

- The Agents panel shows the real overlay with **one completed** worker and the start of its handoff, not several active parallel jobs. Its full `../features/agents-view.png` source remains accessible in the README. The separate `../features/gentle-shell.png` session is retained as a secondary SDD/OpenSpec example, not presented as the ODD first-session walkthrough.
- The Control panel covers Normal, Auto and YOLO only. It is an explanation of their documented boundaries, not a screenshot or a sandbox claim. [Super Yolo](../../yolo-mode.md#super-yolo) is a separate higher-risk mode outside this diagram's scope.
- Existing GIFs, videos, diagrams, screenshots and credits are preserved. The full workspace screenshot is visible without a toggle.

## Reading without the graphics

Product identity, navigation, capability descriptions, commands and permission caveats remain selectable README text. Alt text describes the evidence and distinguishes the explanatory diagram. At phone widths, use that text or the full source images rather than relying on terminal text inside a reduced graphic.
