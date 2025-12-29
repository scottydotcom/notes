```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Winter Christmas Theme</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <div class="container">
      <h1>Happy Holidays!</h1>
      <p>Wishing you a season filled with warmth, comfort, and good cheer!</p>
    </div>
    <canvas id="snowCanvas"></canvas>
    <script src="script.js"></script>
  </body>
</html>
```

```css
body {
  margin: 0;
  padding: 0;
  background-color: #2c3e50;
  color: white;
  font-family: "Arial", sans-serif;
  overflow: hidden;
}

.container {
  position: relative;
  text-align: center;
  padding: 50px;
  z-index: 1;
}

h1 {
  font-size: 3em;
  margin: 0;
}

p {
  font-size: 1.5em;
}
```

```js
const canvas = document.getElementById("snowCanvas");
const ctx = canvas.getContext("2d");

canvas.width = window.innerWidth;
canvas.height = window.innerHeight;

let snowflakes = [];

function createSnowflake() {
  const x = Math.random() * canvas.width;
  const y = Math.random() * canvas.height;
  const radius = Math.random() * 4 + 1;
  const speed = Math.random() * 1 + 0.5;
  snowflakes.push({ x, y, radius, speed });
}

function updateSnowflakes() {
  for (let i = 0; i < snowflakes.length; i++) {
    const flake = snowflakes[i];
    flake.y += flake.speed;

    if (flake.y > canvas.height) {
      flake.y = 0;
      flake.x = Math.random() * canvas.width;
    }
  }
}

function drawSnowflakes() {
  ctx.clearRect(0, 0, canvas.width, canvas.height);
  ctx.fillStyle = "rgba(255, 255, 255, 0.8)";
  for (let flake of snowflakes) {
    ctx.beginPath();
    ctx.arc(flake.x, flake.y, flake.radius, 0, Math.PI * 2);
    ctx.fill();
  }
}

function animate() {
  updateSnowflakes();
  drawSnowflakes();
  requestAnimationFrame(animate);
}

function init() {
  for (let i = 0; i < 100; i++) {
    createSnowflake();
  }
  animate();
}

window.addEventListener("resize", () => {
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;
});

init();
```
