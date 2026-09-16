# Barcelona Vegan Espresso Trip — SVG assets

Open `preview.html` to see everything on the paper background.

## The system

- **Grid and line:** a 24-unit grid, one stroke weight (1.75), square ends and mitred corners.
- **Base form:** the *xamfrà*, the cut corner of Ildefons Cerdà's Eixample blocks. It shapes the markers, the office icon, the plaques and the sticker.
- **One accent:** every mark carries exactly one coloured dot, the *punt volat*. That's the raised dot in Catalan *l·l*, a character only Catalan uses. The "our pick" icon is simply `l·l`.
- **Words:** Catalan, set like a street plaque, with English beneath.
- **Everything is outlined:** there are no fonts, raster images or external files.

## Words and why

| Catalan | English | Note |
|---|---|---|
| MAPA | map | |
| CAFÈ | espresso | the grave accent is correct in Catalan (not *café*) |
| VEGÀ | vegan | masculine form; *vegana* is feminine |
| MIRAR | see & do | "to look"; the guide is about looking, not ticking off |
| SEGONA MÀ | secondhand | literally "second hand" |
| OFICINA | office | |
| LA NOSTRA TRIA | our pick | *tria* = choice, selection |
| ENTRADA | ticket | also "entrance" |
| A PEU | on foot | |
| METRO | metro | |
| MERCAT | market | |
| PLATJA | beach | |
| ANEM A PEU | let's go on foot | the sticker and stencil tag |

**Please have a Catalan speaker check the words before publishing.**

## Colours

Only the given palette is used. Each mark has one accent colour:

- **Coffee:** Gràcia red
- **Vegan:** Encants green
- **See & do:** Sagrada yellow
- **Secondhand:** Poblenou blue
- **Office:** ink with a sea dot
- **Our pick:** red with the l·l

Area plaques and backgrounds use their own area's colour.

## Deliberately left out

- **Landmarks:** no drawn landmarks and no Gaudí shapes.
- **Travel stereotypes:** no suns, palm trees or flamenco.
- **Politics and brands:** no political slogans, no Metro or TMB logo.
- **Gràcia pattern:** it is not a grid. Its streets open into plaças; the Cerdà grid appears only in Poblenou and at the office.

## Folders

```
icons/        12 × icon-*.svg        24px grid
markers/       6 × marker-*.svg      32×40, anchor at bottom centre (16,39)
badges/        9 × badge-*.svg       16px grid, for pills
plaques/      17 × plaque-*.svg      240×96, Catalan + English
backgrounds/   5 × bg-*-pattern.svg  1200×800, preserveAspectRatio slice
sticker/       sticker-anem-a-peu.svg, tag-anem-a-peu.svg
assets.json    palette, category colours, plaque words
```
