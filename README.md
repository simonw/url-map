# url-map

Use URL parameters to generate a map with markers, using Leaflet and OpenStreetMap

Visit it here: https://simonw.github.io/url-map/

## Parameters

To center the map on a specific location, add `?center=lat,lon`. To set the zoom, use `?zoom=8`.

- https://simonw.github.io/url-map/?center=51.49,0&zoom=8

To add markers, use `?marker=lat,lon`. You can pass this multiple times:

- https://simonw.github.io/url-map/?center=51.49,0&zoom=8&marker=51.49,0&marker=51.3,0.2

## Using this with shot-scraper

You can use this tool to create static map images using [shot-scraper](https://shot-scraper.datasette.io/). For example:

```
shot-scraper 'https://simonw.github.io/url-map/?center=51.49,0&zoom=8&marker=51.49,0&marker=51.3,0.2' \
  --retina --width 600 --height 400 --wait 3000
```
Produces this image:

![A map of London with two blue markers](https://user-images.githubusercontent.com/9599/173208299-b44c34f1-887b-48b7-86d8-4038945ec80f.png)
