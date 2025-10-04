<!DOCTYPE html>
<html>
<head>
<style>
  body {
    margin: 0;
    background: #000;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  iframe {
    border: none;
    width: 80vw;
    height: 80vh;
    border-radius: 10px;
  }

  button {
    margin-top: 10px;
    padding: 10px 20px;
    background-color: #ff00ff;
    color: white;
    border: none;
    border-radius: 5px;
    font-size: 16px;
    cursor: pointer;
  }

  button:hover {
    background-color: #ff55ff;
  }
</style>
</head>
<body>

<iframe 
  id="gameFrame"
  src="https://papaspizzeria.io/papas-pizzeria.embed" 
  allowfullscreen>
</iframe>

<button onclick="toggleFullscreen()">Fullscreen</button>

<script>
function toggleFullscreen() {
  const iframe = document.getElementById('gameFrame');

  if (document.fullscreenElement) {
    document.exitFullscreen();
  } else {
    iframe.requestFullscreen().catch(err => {
      alert(`Error attempting fullscreen: ${err.message}`);
    });
  }
}
</script>

</body>
</html>
