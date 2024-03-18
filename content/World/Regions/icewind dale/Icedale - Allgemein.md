reload the page to view the map!



<html> <head> <link href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" rel="stylesheet"/> </head> <body> <div id="map" style="width: 100%; height: 1200px;"></div>  <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script> <script> var map = L.map('map', { crs: L.CRS.Simple, minZoom: -4, maxZoom: 6,  }); var bounds = [[0, 0], [6000, 4215]]; var image = L.imageOverlay('../../../../images/mzinigboq9391.webp', bounds).addTo(map); map.on('load', function() { map.invalidateSize(); }); map.fitBounds(bounds); </script> </body> </html>


