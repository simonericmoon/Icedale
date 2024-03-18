![[014-map-1.1-bremen-player.webp]]



<html>
<div id="map" style="width: 100%; height:1000px ;"></div> <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script> <link href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" rel="stylesheet"/>  <script>   var map = L.map('map', {     crs: L.CRS.Simple,     minZoom: -2,     maxZoom: 7,   });    var bounds = [[0, 0], [3000, 2208]];   var image = L.imageOverlay('../images/014-map-1.1-bremen-player.webp', bounds).addTo(map); map.on('load', function() {     map.invalidateSize();   });    map.fitBounds(bounds); </script>
</html>

