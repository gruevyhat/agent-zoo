# The Agent Zoo

Infographic field guides to LLM agent architectures, in the style of the old neural-network "model zoo" posters. 64 patterns across four volumes.

**View it live:** https://gruevyhat.github.io/agent-zoo/

| File | Contents |
|---|---|
| `index.html` | Landing page linking the three volumes |
| `vol1-classic.html` | Vol. I: Classic species (01–16) |
| `vol2-recent.html` | Vol. II: Recent and exotic species, 2024–2026 (17–32) |
| `vol3-harness.html` | Vol. III: Coding harnesses (33–48) |
| `vol4-multimodal.html` | Vol. IV: Multimodal species (49–64) |
| `canvas/` | Original Claude Design canvas sources (`*.dc.html` + `canvas.json`) |
| `SOURCES.md` | Sources behind each tile in Vols. II–IV |

Open `index.html` in a browser. Each page is a single self-contained HTML file (fonts load from Google Fonts; everything else is inline SVG and CSS), drawn at 1600 px wide.

The live, editable version is a Claude Design canvas with one page per volume. The `canvas/` files are a snapshot of it. The top-level `vol*.html` files are the same artboards with the canvas runtime tags stripped so they open standalone. If you edit the canvas, regenerate these rather than hand-editing both.

## Conventions

- **Glyph legend:** grey = input/output, amber = LLM call, blue square = tool, purple pill = memory/state/files, red ring = critic/gate, ringed dot = human, green box = environment/sandbox, dashed outline = untrusted data or a boundary. Solid edges always fire; dashed edges are conditional.
- **Every tile has a "Breaks when" line.** Some come from the sources; many are editorial judgment. Treat them as prompts for discussion, not findings.
- **Evidence grades (Vols. II–IV):** Peer-reviewed, Preprint + code, Shipped feature (documented product behaviour, not a measured result), Vendor write-up (a lab describing its own system, usually on internal evals), Spec (a standard, not a result), Trend/Practitioner (forecast or folk technique).

## Known gaps

- Vol. I tile text was written from general knowledge without a fresh literature pass.
- Vol. II tile 32 (human-on-the-loop) rests on a second-hand analyst forecast; weakest tile in the set.
- Two Vol. III source strings (Aider edit-formats docs, ghuntley.com/ralph) were not opened directly.
- Vol. IV tile 59 (half-cascade) rests on a second-hand report of a Google claim.
- Rendering has not been checked at every height; the pages are tall and tile text varies.
