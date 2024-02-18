<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>3D Model Rotation with Slider</title>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            background-color: #f0f0f0;
        }
        model-viewer {
            width: 400px;
            height: 400px;
        }
    </style>
</head>
<body>

<model-viewer id="pizzaModel" src="pizza.glb" ios-src="pizza.usdz" ar ar-modes="webxr scene-viewer quick-look" camera-controls auto-rotate environment-image="neutral" shadow-intensity="5" alt="Un modello 3D di pizza"></model-viewer>

<!-- Slider -->
<input type="range" id="modelSlider" min="0" max="360" value="0" style="width: 400px;">

<script>
    const modelViewer = document.getElementById('pizzaModel');
    const slider = document.getElementById('modelSlider');

    slider.addEventListener('input', function() {
        const rotationDegree = this.value;
        // Actualizăm rotația modelului 3D pe axa Y
        modelViewer.style.transform = `rotateY(${rotationDegree}deg)`;
    });
</script>

</body>
</html>
