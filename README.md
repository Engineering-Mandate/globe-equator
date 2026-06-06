# Globe Equator Explorer

An interactive 3D globe for drawing great-circle lines between ancient landmarks and modern cities, then measuring how closely they align.

**[▶ Live demo](https://engineering-mandate.github.io/globe-equator/)**

## What it does

Select two or more landmarks from the sidebar and click **Draw Great-Circle Line**. The app draws a full great circle through those points on the globe and reports, for every landmark, how many degrees it sits off that line. Tight alignments (< 1°) show green; loose ones (> 5°) show red.

Useful for exploring theories about ancient site alignments, ley lines, or just playing with spherical geometry.

## Controls

- **Drag** the globe to rotate
- **Scroll** to zoom
- **Click a landmark** (sidebar or globe dot) to select/deselect it
- **Add Custom Point on Globe** — enter placement mode and click anywhere on the globe to drop a point
- **Clear Selection** — deselect all without removing drawn lines
- Lines can be removed individually with the ✕ on each line card

## Landmarks included

**Ancient sites:** Great Pyramid of Giza, Stonehenge, Easter Island, Machu Picchu, Angkor Wat, Nazca Lines, Petra, Mohenjo-daro, Göbekli Tepe, Teotihuacan, Chichen Itza, Tiwanaku, Nan Madol, Ollantaytambo, Sacsayhuamán

**Modern cities:** New York, London, Paris, Tokyo, Beijing, Sydney, Dubai, Mumbai, São Paulo, Cairo, Moscow, Los Angeles, Singapore, Toronto, Cape Town

## Implementation

Single self-contained `index.html`. Uses [globe.gl](https://globe.gl/) for the 3D rendering. All great-circle math is done in plain JS with vector cross products.
