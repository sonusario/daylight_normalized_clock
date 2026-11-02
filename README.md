# Daylight Clock

**Live:** https://sonusario.github.io/daylight_normalized_clock/

A clock where sunrise is always 6:00 AM and sunset is always 6:00 PM. The hours in between stretch or shrink to fit the real day, so a winter daylight hour is short and a summer one is long.

- Works out sunrise and sunset from your location with the NOAA solar equations.
- Pick a location with your device's location, a place search ("City, state, country"), or by turning the globe until the crosshairs sit on your spot. The nearest big city to the crosshairs is shown as you turn it.
- Two sets of hour, minute and second hands: daylight time and real time. Tap the legend to swap which set is filled and which is a dashed outline. The hour hands read the 24-hour face; minute and second hands read the outer 0 to 60 ring.
- Small triangles on the face mark where the two clocks will agree in the next day.
- Real times use the selected location's time zone (looked up offline from the coordinates), shown with a mini globe in the clock's corner.
- Themes for the hand colors; Portal (orange daylight, blue real time) is the default.
- Installable as an app (PWA) and works offline once it has loaded. Only place searches need the internet.

## Files

- `index.html`: the whole app.
- `sw.js`, `manifest.webmanifest`, `icons/`: the installable-app pieces. Bump `VERSION` in `sw.js` when any file changes.
- `data/land-110m.json`: coastlines from Natural Earth via [world-atlas](https://github.com/topojson/world-atlas).
- `lib/tz-lookup.js`: coordinates to IANA time zone, from [tz-lookup](https://github.com/photostructure/tz-lookup) (CC0).
- `data/cities.json`: cities of 300,000+ people plus national capitals, from [GeoNames](https://www.geonames.org/) (CC BY 4.0).

Part of [Sonusario's Selects](https://sonusario.github.io/).
