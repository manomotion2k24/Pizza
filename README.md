Pizza Quattro Formaggie
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Visualizza modello 3D</title>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
    <style>
      model-viewer {
        width: 100%;
        height: 500px;
      }
      @keyframes levitate {
        0%, 100% {
          transform: translateY(0);
        }
        50% {
          transform: translateY(-10px);
        }
      }
      .levitate {
        display: inline-block;
        animation: levitate 1s ease-in-out infinite;
      }
    </style>
</head>
<body>

<div style="padding: 20px; text-align: center;">
    <h2>Ingredienti per la pizza:</h2>
    <p>100 g di formaggio grattugiato stagionato vaccino.<br>
    100 g di Pecorino grattugiato.<br>
    80 g di ricotta.<br>
    40 g di Gorgonzola.<br>
    1 rametto di rosmarino.<br>
    10 foglie di origano.<br>
    40 g di Parmigiano.<br>
    2 cucchiai di olio d'oliva.</p>
</div>

<model-viewer src="pizza.glb" ios-src="pizza.usdz" ar ar-modes="webxr scene-viewer quick-look" camera-controls auto-rotate environment-image="neutral" shadow-intensity="1" alt="Un modello 3D di pizza">
  <button slot="ar-button" class="ar-button" style="background-color: white; border-radius: 4px; border: none; position: absolute; top: 16px; right: 16px; ">
      <span class="levitate">👋</span> Activează modul AR
  </button>
</model-viewer>

</body>
</html>
