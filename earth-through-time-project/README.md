# Earth Through Time — project folder

This folder contains the interactive globe, its source data, and the map assets used by the project.

## Run it

Because the app uses JavaScript modules, open it from a small local web server instead of double-clicking the file. On macOS, open Terminal in this folder and run:

```sh
python3 -m http.server 8000
```

Then visit <http://localhost:8000/>. The globe, country borders, ancient reconstructions, terrain data, and bundled map libraries are local. Country photos and additional English/Turkish species-name lookups are loaded from Wikimedia Commons and GBIF while online.

## What is included

- `index.html` — editable app source and runnable page, including a compressed copy of the modern country map.
- `data/earth-history.json` — full data payload: 21 reconstructed time snapshots, 177 country profiles, 416 terrain regions, 60 terrain peaks, and 12 natural-event groups.
- `maps/countries-110m.json` — modern country-boundary TopoJSON used by the globe.
- `vendor/d3-geo.mjs` and `vendor/topojson-client.mjs` — local copies of the map-rendering modules.
- `SOURCES.md` — data sources and runtime network notes.

The standalone export remains available separately in the outputs folder.
