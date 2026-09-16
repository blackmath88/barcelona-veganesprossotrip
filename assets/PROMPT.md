# Prompt for Codex / Claude Code: integrate the SVG assets

Paste everything below the line into the coding agent at the repo root. Put the unzipped `assets/` folder next to `index.html` first.

---

Integrate the SVG set in `assets/svg/` into this static Barcelona guide (`index.html`, GitHub Pages). Read `assets/svg/LLEGEIX-ME.md` first.

Constraints:
- No build step and no new dependencies. Keep it one HTML file plus the SVG files.
- Leave all copy and layout unchanged except the steps below.
- Decorative images get `alt=""`. Plaques that replace a text label get `alt` with the Catalan and English words.

Steps:
1. **Palette.** Replace the CSS tokens with the palette from `assets/svg/assets.json`:
   - `--paper #E8E0D4`, `--ink #151515`, `--muted #5C5851`
   - `--coffee` → `#E45E40`, `--vegan` → `#6F9C88`, `--look` → `#E5B83F`, `--love` → `#E45E40`, `--sea` → `#2C94B8`
   - Update the `colors` object in the script to match.
2. **Map markers.** In `iconFor()`, replace the CSS div marker with an `<img>` of `assets/svg/markers/marker-<cat>.svg`:
   - Category mapping: coffee → coffee, vegan → vegan, look → see-do. Personal picks use `marker-favorite.svg`.
   - Set `iconSize [26,32]`, `iconAnchor [13,31]`, `popupAnchor [0,-28]`.
3. **Filter buttons and nav.** Add the matching 14px icon before each label: map, coffee, vegan, see-do. "Our picks" gets `icon-favorite`.
4. **Pills and cards.** In `.pill` and `.cat`, add the 12px badge: espresso, vegan, architecture or browse. Replace the "♥ OUR PICK" / "♥ PERSONAL PICK" heart with `badge-our-pick.svg`.
5. **Numbered sections.** Use the backgrounds at low strength (`opacity .5` via a pseudo-element):
   - 01 Gràcia → `bg-gracia-pattern.svg`
   - 02 Trafalgar → `bg-office-pattern.svg`
   - 03 Sagrada → `bg-sagrada-pattern.svg`
   - 04 Encants → `bg-encants-pattern.svg`, plus `bg-poblenou-pattern.svg` in the lower half if it fits
6. **Section plaques.** Put the area plaque (`plaque-gracia.svg`, etc.) above each numbered heading at 200px wide.
7. **Sticker.** Place `sticker/sticker-anem-a-peu.svg` in the landing hero:
   - absolutely positioned, top right, about 220px wide, rotated a few degrees
   - hidden below 700px
   - put `sticker/tag-anem-a-peu.svg` in the dark "No La Rambla day" block, about 360px wide

Verify: open the page, check the map markers, filters and all four sections on desktop and mobile widths, and confirm there are no console errors or missing files.
