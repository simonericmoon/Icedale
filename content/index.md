---
title: "Willkommen zur Lore-Seite der DnD Kampagne: Icewind Dale: Rime of the Frostmaiden!"
---
Hier die [[Abenteuerbeschreibung]]!
![[ai-created-image-for-rime-of-the-frostmaiden-v0-aip9b72ttyqa1.webp]]

Hier findest du alle Informationen zur Kampagne - kennengelernte NPC's, besuchte Orte und Hintergrundwissen der Welt. Bei Fragen, Anmerkungen gerne bei mir melden! (:

Diese Kampagne ist WIP.

Author: Simon E. K.
ysbfh96bj1s51.webp

<html>
<div id="map" style="width: 90%; height: 250px;"></div>

<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"></script>

<link href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" rel="stylesheet"/>

  

<script>

var map = L.map('map', {

crs: L.CRS.Simple,

minZoom: -2,

maxZoom: 2,

});

  

var bounds = [[0, 0], [900, 2279]];

var image = L.imageOverlay('ysbfh96bj1s51.webp', bounds).addTo(map);

map.fitBounds(bounds);

  
  

</script>
</html>





























