<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3D Model View with Interactive Heart</title>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
    <style>
      @keyframes fall {
        to { transform: translateY(100vh); }
      }
      .heart {
        position: fixed;
        top: -100px;
        color: red;
        animation: fall linear;
      }
      .big-heart {
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        font-size: 100px;
        color: red;
        display: none;
        z-index: 1000;
      }
      model-viewer {
        width: 100%;
        height: 500px;
      }
      @keyframes levitate {
        0%, 100% {
          transform: translateY(0);
        }
        50% {
          transform: translateY(-5px);
        }
      }
      .levitate {
        display: inline-block;
        animation: levitate 1s ease-in-out infinite;
      }
      .recipe-text {
        padding: 20px;
        text-align: center;
      }
    </style>
</head>
<body>

<model-viewer 
    ar 
    camera-controls 
    touch-action="pan-y" 
    src="pizza.glb" 
    ios-src="pizza.usdz" <!-- Adăugat suport pentru .usdz -->
    alt="A 3D model of pizza">
  <button slot="ar-button" class="ar-button" style="background-color: white; border-radius: 4px; border: none; position: absolute; top: 16px; right: 16px;">
      <span class="levitate">👋</span> Activează modul AR
  </button>
</model-viewer>

<div class="recipe-text">
  100 g di formaggio grattugiato stagionato vaccino.<br>
  100 g di Pecorino grattugiato.<br>
  80 g di ricotta.<br>
  40 g di Gorgonzola.<br>
  1 rametto di rosmarino.<br>
  10 foglie di origano.<br>
  40 g di Parmigiano.<br>
  2 cucchiai di olio d'oliva.
</div>

<div id="touchHeart" class="big-heart">❤️</div>

<script>
  // Script pentru crearea inimioarelor și logica pentru inima mare așa cum a fost descris anterior
</script>

</body>
</html>
