<html>
<head>
<p><span style="font-family: verdana; color: #ff00ff;"><strong>More will be added one day XD, this is just a test for my github page :D</strong></span></p>
<p><img class="post__image align-right" src="https://raw.githubusercontent.com/meowseal/meowseal.github.io/2c37ecdc46d9a32e59cdbdaef3fb403463a0f586/harp-seal-pup.webp" alt="" width="437" height="328"></p>
<p>Anyways heres papas pizzaria</p>

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
    background-color: #dd55dd;
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
