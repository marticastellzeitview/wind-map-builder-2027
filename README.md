# GE · ES/PT · TEST — local replica

This folder contains a local copy of the interactive map and its CSV/XLSX map creator from https://ge-testmap.pages.dev/.

## Open it

Serve this folder over HTTP so the map can load its companion files. From this folder, run:

```sh
python3 -m http.server 8000
```

Then open http://localhost:8000/create/ to upload a turbine spreadsheet. The creator detects common column names, lets you adjust the mapping, checks the rows, and creates a shareable map link. Open http://localhost:8000/ to view the reference map.

CSV files can use the included “Download the template” link as a starting point. The creator also accepts Excel `.xlsx` files, files with one row per turbine, and files with one row per blade.

The farm register and map geometry are included locally. Satellite imagery, weather, place search, and driving routes use the same public online services as the reference and need an internet connection.
