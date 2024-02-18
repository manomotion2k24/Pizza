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

</body>
</html>
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
	background-image: linear-gradient(45deg, #223, #112);
  background:
    radial-gradient(at 100% 0, #fff2, #fff0 50%),
    radial-gradient(at 0% 100%, #0002, #0000 50%),
    #545153;
}

/* 

styles based on this guide: 
 - https://www.smashingmagazine.com/2021/12/create-custom-range-input-consistent-browsers/

design based on these demos: 
  - https://codepen.io/alvaromontoro/pen/yLwPvaG
  - https://codepen.io/jh3y/pen/YzgYPNb

*/
/* this property may not be needed as we update based on --val */
@property --c {
  syntax: '<color>';
  inherits: true;
  initial-value: #0000;
}


.glow {
  --c: rgb(0, 255, 255, calc(0.25 + var(--val) / 125));
  --c: hsl(160deg 80% 50% / calc(0.25 + var(--val) / 125));
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  background: transparent;
  cursor: pointer;
  width: 15rem;
  position: relative;
}

.glow::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: calc((var(--val) - 1) * 1%);
  min-width: 0.5em;
  height: 100%;
  background: var(--c);
  box-shadow: 
    0 0 0.2em 0 hsl(0 0% 0%) inset, 
    -0.1em 0.1em 0.1em -0.1em hsl(0 0% 100% / 0.5),
    0 0 calc(1em + 0.001em * var(--val)) calc(0.1em + 0.00025em * var(--val)) var(--c)
    ;
  border-radius: 1em 0 0 1em;
  aopacity: calc(20% + var(--val) * 1%);
}

/***** Track Styles *****/
/***** Chrome, Safari, Opera, and Edge Chromium *****/
.glow::-webkit-slider-runnable-track {
  box-shadow: 
    0 0 0.2em 0 hsl(0 0% 0%) inset, 
    -0.1em 0.1em 0.1em -0.1em hsl(0 0% 100% / 0.5);
  background: 
    linear-gradient(to bottom right, #0001, #0000),
    #343133;
  border-radius: 1em;
  height: 1em;
}

/******** Firefox ********/
.glow::-moz-range-track {
  box-shadow: 0 0 2px 0 hsl(0 0% 0%) inset, -1px 1px 1px -1px hsl(0 0% 100% / 0.5);
  background: 
    linear-gradient(var(--c) 0 0) 0 0 / calc(var(--val) * 1%) 100% no-repeat,
    linear-gradient(to bottom right, #0001, #0000),
    #343133;
  border-radius: 1em;
  height: 1em;
}


/***** Thumb Styles *****/
/***** Chrome, Safari, Opera, and Edge Chromium *****/
.glow::-webkit-slider-thumb {
  --d: var(--c);
  --d: rgb(from var(--c) r g b / calc(0.35 * var(--val) * 1%));
  -webkit-appearance: none; /* Override default look */
  appearance: none;
  background-color: #5cd5eb;
  transform: translateY(calc(-50% + 0.5em));
  width: 4em;
  aspect-ratio: 1;
  background: red;
  border-radius: 50%;
  background: 
    radial-gradient(farthest-side, #0000 22.5%, var(--d) 0, #0000 calc(var(--val) * 0.75%)) 50% 50% / 100% 100% no-repeat,
    radial-gradient(#0000  15%, #343133 16%, #545153 20%),
    repeating-linear-gradient(#0000 0 10%, #0002 0 20%) 50% 50% / 25% 25% no-repeat,
    repeating-linear-gradient(90deg, #0000 0 10%, #0002 0 20%) 50% 50% / 25% 25% no-repeat,
    radial-gradient(var(--c) 17%, #0000 0),
    #545153;
  box-shadow:
    inset -0.15em -0.15em 0.2em #0008,
    inset 0.15em 0.15em 0.2em #ffffff22,
    inset calc(var(--val) * 1em / 500) 0em calc(var(--val) * 1em / 500) calc(var(--val) * -1em / 700) var(--c),
    0.25em 0.25em 0.5em #0006,
    calc(0.0125em * var(--val)) calc(0.005em * var(--val)) calc(0.02em * var(--val)) calc(-0.01em * var(--val)) #000a;
  border-radius: 50%;
    
}

/***** Firefox *****/
.glow::-moz-range-thumb {
/*   --d: var(--c);
  --d: rgb(from var(--c) r g b / calc(0.35 * var(--val) * 1%)); */
  border: none; /*Removes extra border that FF applies*/
  -webkit-appearance: none; /* Override default look */
  appearance: none;
  background-color: #5cd5eb;
  width: 4em;
  height: 4em;
  aspect-ratio: 1;
  background: red;
  border-radius: 50%;
  background: 
/*     radial-gradient(farthest-side, #0000 22.5%, var(--d) 0, #0000 calc(var(--val) * 0.75%)) 50% 50% / 100% 100% no-repeat, */
    radial-gradient(#0000  15%, #343133 16%, #545153 20%),
    repeating-linear-gradient(#0000 0 10%, #0002 0 20%) 50% 50% / 25% 25% no-repeat,
    repeating-linear-gradient(90deg, #0000 0 10%, #0002 0 20%) 50% 50% / 25% 25% no-repeat,
    radial-gradient(var(--c) 17%, #0000 0),
    #545153;
  box-shadow:
    inset -0.15em -0.15em 0.2em #0008,
    inset 0.15em 0.15em 0.2em #ffffff22,
    inset calc(var(--val) * 1em / 500) 0em calc(var(--val) * 1em / 500) calc(var(--val) * -1em / 700) var(--c),
    0.25em 0.25em 0.5em #0006,
    calc(0.015em * var(--val)) calc(0.005em * var(--val)) calc(0.02em * var(--val)) calc(-0.01em * var(--val)) #0008;
  border-radius: 50%;
}
