
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

<html> <head> <title>Interactive Fantasy Map</title> <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" /> <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script> </head> <body> <div id="map" style="width: 600px; height: 400px;"></div> <script> var map = L.map('map').setView([0, 0], 2); L.tileLayer('../images/ysbfh96bj1s51.webp', { maxZoom: 10, minZoom: 1, noWrap: false, worldCopyJump: false, bounds: [[-90, -180], [90, 180]], }).addTo(map); </script> </body> </html>

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


<div class="zoomable-image">
  ![Your Image Description](../images/ysbfh96bj1s51.webp)
</div>


<html>
<div id="imageContainer" style="overflow:hidden; width:500px; height:300px;">
    <img id="zoomableImage" src="../images/ysbfh96bj1s51.webp" style="width:100%; cursor:grab;">
</div>
<style>
#imageContainer {
    /* Adjust these values as needed */
    width: 500px; 
    height: 300px;
    overflow: hidden;
}

#zoomableImage {
    width: 100%;
    cursor: grab;
    transition: transform 0.25s ease;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function() {
    let img = document.getElementById('zoomableImage');
    let container = document.getElementById('imageContainer');
    let posX = 0, posY = 0, scale = 1;
    let lastPosX = 0, lastPosY = 0, lastScale = 1;

    img.onwheel = function(e) {
        e.preventDefault();
        scale = Math.max(1, Math.min(lastScale + (e.deltaY * -0.01), 4));
        img.style.transform = `translate(${lastPosX}px, ${lastPosY}px) scale(${scale})`;
    };

    let isDragging = false;

    img.onmousedown = function(e) {
        e.preventDefault();
        isDragging = true;
        posX = e.clientX - lastPosX;
        posY = e.clientY - lastPosY;
        container.style.cursor = 'grabbing';
    };

    document.onmousemove = function(e) {
        if (isDragging) {
            lastPosX = e.clientX - posX;
            lastPosY = e.clientY - posY;
            img.style.transform = `translate(${lastPosX}px, ${lastPosY}px) scale(${scale})`;
        }
    };

    document.onmouseup = function(e) {
        isDragging = false;
        container.style.cursor = 'grab';
    };
});
</script>
</html>

