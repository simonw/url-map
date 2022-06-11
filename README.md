# url-map

Use URL parameters to generate a map with markers, using Leaflet and OpenStreetMap

Visit it here: https://simonw.github.io/url-map/

## Parameters

To center the map on a specific location, add `?center=lat,lon`. To set the zoom, use `?zoom=8`.

- https://simonw.github.io/url-map/?center=51.49,0&zoom=8

To add markers, use `?marker=lat,lon`. You can pass this multiple times:

- https://simonw.github.io/url-map/?center=51.49,0&zoom=8&marker=51.49,0&marker=51.3,0.2
