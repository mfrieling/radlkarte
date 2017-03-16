# radlkarte.at

online map with the goal to provide useful (route) information for cyclists

## Features
- show recommended bicycle routes
  - three quality types of route segments: calm, medium, stressful
  - three importance levels of route segments: main, regional, local
    - hide parts of the recommended routes when zooming out
  - oneway arrow for route segments only usable in one direction
- GPS localization (especially useful for mobile devices)
- geocoding with OSM (nominatim)

### Future Work
- highlighting of short parts where bicycle has to be pushed & dangerous crossings
- optional overlays for cycling-POIs such as citybike stations or bicycle shops
- differentiate between a simple & an advanced UI.
  - simple: auto-hides parts of the network based on zoom level, no layer switcher
  - advanced: layer switcher, control opacity of overlay, freely choose network-parts to show
- add basemap.at as background layer?
- nicer opacity? not possible with current approach: https://github.com/Leaflet/Leaflet/issues/3610
  but maybe just add the background layer on top again with high opacity?

## Notes

linting:
    jshint radlkarte.js
    /usr/local/lib/node_modules/html5-lint/html5check.py index.html
