# Daylight Clock

**Live:** https://sonusario.github.io/daylight_normalized_clock/

A clock where sunrise is always 6:00 AM and sunset is always 6:00 PM. The hours in between stretch or shrink to fit the real day, so a winter daylight hour is short and a summer one is long.

- Works out sunrise and sunset from your location with the NOAA solar equations.
- Pick a location with your device's location, a place search ("City, state, country"), or by turning the globe until the crosshairs sit on your spot. The nearest big city to the crosshairs is shown as you turn it.
- Installable as an app (PWA) and works offline once it has loaded. Only place searches need the internet.

## Files

- `index.html`: the whole app.
- `sw.js`, `manifest.webmanifest`, `icons/`: the installable-app pieces. Bump `VERSION` in `sw.js` when any file changes.
- `data/land-110m.json`: coastlines from Natural Earth via [world-atlas](https://github.com/topojson/world-atlas).
- `data/cities.json`: cities of 300,000+ people plus national capitals, from [GeoNames](https://www.geonames.org/) (CC BY 4.0).

Part of [Sonusario's Selects](https://sonusario.github.io/).
