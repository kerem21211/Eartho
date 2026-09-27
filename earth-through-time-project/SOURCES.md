# Data and code sources

- **Modern country boundaries:** `@d3-maps/atlas` world countries, 110m resolution, version 1.0.0. The TopoJSON is included at `maps/countries-110m.json` and embedded in `index.html`.
- **Ancient coastlines and continent positions:** reconstructed GeoJSON snapshots and model identifiers are included in `data/earth-history.json`; the app cites GPlates reconstruction models and records the model used per snapshot.
- **Terrain regions and peaks:** geometry is included in `data/earth-history.json`; the app credits Natural Earth physical-feature data.
- **Geologic periods:** period boundaries follow the International Commission on Stratigraphy chart; period summaries are in `index.html`.
- **Country fauna and flora records:** species lists are included in `data/earth-history.json`. GBIF is the linked source for occurrence and vernacular-name records.
- **Country photographs:** loaded on demand from Wikimedia Commons. The interface links to each image page and displays the file creator and license when Commons provides them; photos are not copied into this folder.
- **Bundled libraries:** `d3-geo` 3.1.1 and `topojson-client` 3.1.0 are local ES module bundles in `vendor/`; license notices for them and the atlas map package are in `vendor/licenses/`.

## Live connections

The page can draw its globe, country map, ancient reconstructions, and terrain from local files. It needs internet access for Commons photos and fresh GBIF common-name lookups. The app has fallbacks when either service is unavailable.
