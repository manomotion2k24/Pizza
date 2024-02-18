<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Comandă acum prin Glovo: Pizzeria Celentano Timișoara</title>
    <script type="module" src="https://unpkg.com/@google/model-viewer"></script>
    <style>
      body {
        margin: 0; /* Asigură-te că nu există margini implicite */
        padding: 0; /* Elimină orice padding implicit */
      }
      model-viewer {
        width: 100%;
        height: 250px;
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
      .ar-button {
        background-color: white;
        border-radius: 4px;
        border: none;
        position: absolute;
        top: 8px;
        right: 8px;
      }

      h2 {
        font-size: 100%; /* Păstrează titlul de 2 ori mai mic */
        margin: -20px 0 0 0; /* Mută titlul mai sus prin aplicarea unui margin negativ */
      }
      h3 {
        font-size: 150%; /* Face textul "Pizza Quattro Formaggi" mai mare */
        font-weight: bold; /* Îngroașă textul */
        margin: 20px 0 10px 0; /* Adaugă un spațiu deasupra și sub titlul secțiunii */
      }
      p {
        font-size: 100%; /* Face textul cu ingrediente puțin mai mic */
      }
      /* Stil pentru hyperlink-ul îngroșat */
      .bold-link {
        font-weight: bold; /* Îngroașă textul */
      }
    </style>
</head>
<body>

<div style="text-align: left; padding: 15px;">
    <h2><a href="https://glovoapp.com/ro/ro/timisoara/pizzeria-celentano-timisoara-tim/" target="_blank">Comandă acum prin Glovo: Pizzeria Celentano Timișoara</a></h2>
    <h3>Pizza Quattro Formaggi</h3>
    <model-viewer src="pizza.glb" ios-src="pizza.usdz" ar ar-modes="webxr scene-viewer quick-look" camera-controls auto-rotate environment-image="neutral" shadow-intensity="5" alt="Un modello 3D di pizza" min-camera-orbit="auto 45deg auto" max-camera-orbit="auto 90deg auto">
      <button slot="ar-button" class="ar-button">
          <span class="levitate">👋</span> Activează modul AR
      </button>
    </model-viewer>
    <p>100 g di formaggio grattugiato stagionato vaccino.<br>
    100 g di Pecorino grattugiato.<br>
    80 g di ricotta.<br>
    40 g di Gorgonzola.<br>
    1 rametto di rosmarino.<br>
    10 foglie di origano.<br>
    40 g di Parmigiano.<br>
    2 cucchiai di olio d'oliva.</p>
    <!-- Hyperlink adăugat sub lista de ingrediente -->
    <p><a href="https://manomotion2k24.github.io/ManoTheQRking/" class="bold-link" target="_blank">Nike Free Matcon</a></p>
     <p><a href="https://manomotion2k24.github.io/cactus/" class="bold-link" target="_blank">Cactus Opuntia Albispina</a></p>
</div>

body {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 3rem;
  overflow: hidden;
  margin: 0;
  min-height: 100vh;
  box-sizing: border-box;
  background: linear-gradient(45deg, #223, #112), 
    radial-gradient(at 100% 0, #fff2, #fff0 50%), 
    radial-gradient(at 0% 100%, #0002, #0000 50%), 
    #545153;
}

@property --val {
  syntax: '<number>';
  inherits: false;
  initial-value: 50;
}

.glow {
  --val: 50; /* Valoarea inițială a slider-ului */
  width: 15rem; /* Lățimea slider-ului */
  height: 2em; /* Înălțimea slider-ului */
  position: relative;
  background: transparent;
  cursor: pointer;
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
}

.glow::-webkit-slider-runnable-track,
.glow::-moz-range-track {
  box-shadow: 0 0 0.2em 0 hsl(0 0% 0%) inset, -0.1em 0.1em 0.1em -0.1em hsl(0 0% 100% / 0.5);
  background: linear-gradient(to bottom right, #0001, #0000), #343133;
  border-radius: 1em;
  height: 1em;
}

.glow::-webkit-slider-thumb,
.glow::-moz-range-thumb {
  -webkit-appearance: none;
     -moz-appearance: none;
          appearance: none;
  width: 2em; /* Diametrul butonului slider-ului */
  height: 2em; /* Diametrul butonului slider-ului */
  background-color: #5cd5eb; /* Culoarea butonului slider-ului */
  border-radius: 50%;
  cursor: pointer;
  /* Ajustează stilurile de mai jos pentru a personaliza aspectul */
  box-shadow: 0 0 0.5em 0.1em rgba(0, 255, 255, 0.5);
}

/* Stiluri suplimentare pentru aspectul dorit pot fi adăugate aici */
