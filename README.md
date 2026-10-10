# Die Vakuole · The Vacuole

An interactive study page about the plant vacuole, built around a real-time 3D model of a plant cell. The page is available in German and English.

**Live:** https://kingkimabdu.github.io/VAKUOLE.github.io/

**Deutsch:** Eine interaktive Lernseite zur Vakuole der Pflanzenzelle mit einem 3D-Modell, das zeigt, wie die Vakuole Ionen aufnimmt, Wasser zieht, Turgor aufbaut und bei Plasmolyse wieder Wasser verliert.

## What's on the page

- **Plate I · the model.** A three.js plant cell with cell wall, cell membrane, central vacuole (tonoplast and cell sap), nucleus, chloroplasts and mitochondria streaming around the cell (cyclosis). Proton pumps (H⁺), ion transporters (K⁺, Cl⁻) and aquaporins sit on the tonoplast.
- **Four stages**, played in sequence or chosen directly:
  1. **Ions flow in:** proton pumps acidify the cell sap and transporters load K⁺ and Cl⁻ into the vacuole. Anthocyanin turns redder as the pH drops; pressure and volume stay put until water moves.
  2. **Water follows (osmosis):** water enters through aquaporins; the vacuole grows and presses the cytoplasm against the wall.
  3. **Turgor:** the wall holds against about 8 bar of internal pressure.
  4. **Plasmolysis:** the cell sits in a salt solution (Na⁺, Cl⁻) more concentrated than the cell sap. Water leaves, the ions stay, and the protoplast pulls away from the wall.
- **Live readouts** for turgor pressure, vacuole volume and cell-sap pH.
- **Numbered key:** hover a number (or focus it with the keyboard) to isolate that part of the model. During each stage, the parts that aren't involved fade back.
- **Reading sections:** structure, functions, types and occurrence, a second plate comparing plant and animal cells, a comparison table, and eight cited sources.
- **DE / EN switch** in the header. The choice is remembered, and the first visit follows the browser language.

## Controls

| Action | Mouse / keyboard | Touch |
| --- | --- | --- |
| Rotate | drag | one-finger drag |
| Zoom | Ctrl + scroll | pinch |
| Play / pause | "Modell starten" button | tap |
| Jump to a stage | stage rail under the model | tap |
| Highlight a part | hover or Tab through the key | tap a key entry (tap again to clear) |

Normal scrolling over the model keeps scrolling the page; zooming needs Ctrl (or a pinch) on purpose.

## Run it

It is one static HTML file. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
# then open http://localhost:8000/
```

The model loads three.js (v0.169) and two Google Fonts (Bricolage Grotesque, Atkinson Hyperlegible Next) from CDNs, so it needs an internet connection. Without WebGL, the page shows a notice and all the text content still works.

## Accessibility

- WCAG AA contrast across the dark green plates and reading pages.
- Keyboard-operable stage rail, buttons, language switch and key.
- `prefers-reduced-motion`: no auto-rotation or streaming, and stages snap to their end state.

## Accuracy note

The model is strongly simplified and not to scale; the pressure and pH values are typical orders of magnitude, not measurements. The content is based on the sources listed on the page (u-helmich.de, Spektrum Lexikon der Biologie, StudySmarter, Studyflix, Pflanzenforschung.de, abitur-wissen.org).

## License

MIT, see [LICENSE](LICENSE).

## Author

© Abdullah Alhariri (KINGKIMABDU). Also by me: [Die Mitose, an interactive mitosis simulation](https://kingkimabdu.github.io/MITOSIS/).
