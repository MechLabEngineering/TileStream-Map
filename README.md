TileStream-Map
==============

Delivers a Map from .mbtiles file from local Server


## Get the Map online

1. Create a map with [TileMill](https://www.mapbox.com/tilemill/) and export as `.mbtiles` file.
2. copy local `.mbtiles` file to server with `scp <mymap>.mbtiles <user>@<server-adress>.de:/path/to/mymap/`
3. get [TileStream](https://github.com/mapbox/tilestream) up and running
    `tilestream --tiles=/path/to/mymap`
4. clone the `index.html` to a server path, go to this directory
5. start a HTTP server to answer requests from web
    e.g. `python -m SimpleHTTPServer 8080`
    
Now your own Tile Server is up and running to provide a map online out of a `.mbtiles` file.
