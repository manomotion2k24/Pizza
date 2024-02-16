Pizza Quattro Formaggi
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

<model-viewer src="pizza.glb" ios-src="pizza.usdz" ar ar-modes="webxr scene-viewer quick-look" camera-controls auto-rotate environment-image="neutral" shadow-intensity="1" alt="Un modello 3D di pizza"></model-viewer>

</body>
</html>

