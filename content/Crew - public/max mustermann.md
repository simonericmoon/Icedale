
---
title: Max Mustermann
draft: false
tags:
  - mensch
  - Krieger
  - samplePlayer
---

Dies ist ein Beispiel für ein Spieler-Charakter. Die ```Personalquest und backstory``` wird nur dann hier veröffentlicht wenn, der Spieler dies möchte und die anderen Spieler davon wissen! 


## Appearence

<div style="display: flex; align-items: center;">
  <img src="../images/862421d9b2f00ab5705467ca4f66b3b6.jpg" alt="Descriptive text for the image" style="width: 30%; height: auto;"/>
  <p style="margin-left: 20px;">Max Mustermann ist ein 40 Jahre alter Mensch.  Er ist 1,80 groß, trägt eine schwere eiserne Rüstung. Er ist nach Icedale gegangen um besondere Fische zu sammeln. </p>
</div>


<html>
<head>
    <title>Interactive Fantasy Map</title>
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
</head>
<body>
    <div id="map" style="width: 600px; height: 400px;"></div>
    <script>
        var map = L.map('map', {
            minZoom: 1,
            maxZoom: 4,
            center: [0, 0],
            zoom: 1,
            crs: L.CRS.Simple,
            noWrap: true,
            worldCopyJump: false,
        });

        // Assuming your image is 1024x1024 pixels at zoom level 1
        // Adjust these values based on your actual image size and desired zoom levels
        var bounds = [[0, 0], [2279, 900]];

        // Add the image overlay to the map setting bounds
        L.imageOverlay('../images/ysbfh96bj1s51.webp', bounds).addTo(map);

        // Set the view to the center of the image
        map.setView([512, 512], 1);

        // Restrict the view to the image bounds
        map.setMaxBounds(bounds);
    </script>
</body>
</html>


'../images/ysbfh96bj1s51.webp
## Rank
Level: 1 <br>
Ansehn TenTowns: 0
## Personalquest
Max Mustermann ist beauftragt worden um Fische für den König zu sammeln. 
Max ist ein Ritter des Lords Thomas. Er geht nach [[Bremen]].
## Backstory
Soldat <br>
Er gehörte zur Leibgarde des Grafen von Baldurs Gate. 
## noteworthy items

- Großschert mit Rubin 

