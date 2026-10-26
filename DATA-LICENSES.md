# Geographic data: credits, sources and licensing

## OpenStreetMap

**© OpenStreetMap contributors.** OpenStreetMap data is available under the
Open Data Commons Open Database License, **ODbL 1.0**:

- Copyright and attribution: https://www.openstreetmap.org/copyright
- License: https://opendatacommons.org/licenses/odbl/1-0/
- Human-readable summary: https://opendatacommons.org/licenses/odbl/summary/

The OSM extracts (`data/*-source.json`, excluding Natural Earth files),
`data/rivers-osm-api.json`, `data/river-polygons.geojson`, and the derived OSM
geometry in `data/game-data.json` and `index.html` retain the ODbL license.
The compiled geographic database is distributed under ODbL 1.0. Included
source extracts and build scripts allow inspection and regeneration of this
version's adapted geographic data. MIT licensing of original software does
not override attribution or database share-alike obligations. Consult the
license for the distinction between a database and a produced work.

Street and building extracts: OpenStreetMap via Overpass:
https://overpass-api.de/api/interpreter

Additional water geometry: OSM API 0.6 map requests and full relations:
https://www.openstreetmap.org/api/0.6/

- Paris water polygon: https://www.openstreetmap.org/relation/2191006
- Rome water polygon: https://www.openstreetmap.org/relation/5071

The city extracts were retrieved for this prototype on 2026-10-25. OSM base
timestamps are retained where returned by Overpass. These are limited,
static central-district extracts, not complete city maps or live updates.
Coordinates, clipped geometries and estimated heights/widths are not
survey-grade measurements. No Google Maps tiles, satellite imagery, textures
or proprietary city models are included.

## Natural Earth

Natural Earth geographical data is in the **public domain**:
https://www.naturalearthdata.com/about/terms-of-use/

World boundaries:
https://raw.githubusercontent.com/nvkelso/natural-earth-vector/master/geojson/ne_110m_admin_0_countries.geojson

River centerlines:
https://raw.githubusercontent.com/nvkelso/natural-earth-vector/master/geojson/ne_10m_rivers_lake_centerlines.geojson

Local files: `data/world-source.geojson` and
`data/rivers-naturalearth.geojson`. Derived country outlines and generalized
river buffers are embedded in the compiled database. Natural Earth supplies
generalized cartography, not a legal or necessarily current boundary record.

## Original software and other assets

Original game code and interface: `LICENSE-CODE.txt` (MIT).
No external runtime library, web font, audio or image asset is required.
Building selection icons use Unicode emoji rendered by the user's operating
system; no separate emoji image collection is redistributed. Playwright is
a development-only test dependency, not bundled into the standalone game.
