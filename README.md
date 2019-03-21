# Novy_textovy_dokument
<html>
<script src="https://aframe.io/releases/0.6.0/aframe.min.js"></script>
<script src="https://jeromeetienne.github.io/AR.js/aframe/build/aframe-ar.js"></script>
<body style='margin : 0px; overflow: hidden;'>
  <a-scene embedded arjs='sourceType: webcam;'>
    <!-- handle marker with your own pattern -->
    <a-marker type='pattern' url='path/to/pattern-marker.patt'>
      <a-box position='0 0.5 0' material='color: red;'></a-box>
    </a-marker>

    <!-- handle marker with hiro preset -->
    <a-marker preset='hiro'>
      <a-box position='0 0.5 0' material='color: green;'></a-box>
    </a-marker>

    <!-- handle barcode marker -->
    <a-marker type='barcode' value='5'>
      <a-box position='0 0.5 0' material='color: blue;'></a-box>
    </a-marker>

    <!-- add a simple camera -->
    <a-entity camera></a-entity>
  </a-scene>
</body>
</html>
