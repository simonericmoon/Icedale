


<html>
<script src="https://unpkg.com/panzoom/dist/panzoom.min.js"></script>

<div style="display: flex; align-items: center;">
  <div id="panzoom-element" style="width: 80%; overflow: hidden; cursor: grab;">
    <img src="../images/019-map-1.2-bryn-shander-player.webp" alt="Descriptive text for the image" style="width: 100%; height: auto;"/>
  </div>
  <p style="margin-left: 20px;">
    Max Mustermann ist ein 40 Jahre alter Mensch.  Er ist 1,80 groß, trägt eine schwere eiserne Rüstung. Er ist nach Icedale gegangen um besondere Fische zu sammeln.
  </p>
</div>
<script> const element = document.getElementById('panzoom-element'); panzoom(element, { bounds: true, boundsPadding: 0.1 }); </script>
</html>


