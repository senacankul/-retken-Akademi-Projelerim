[Uploadin<!doctype html>

<html>
  <head>
    <link rel="stylesheet" href="lib/style.css">
    <script src="lib/script.js"></script>
    <style>
      h1 { color: white; font-family: 'Papyrus'; font-size: 40px; } body { background-color: purple; } div#kutuResim { width: 930px; height: 1570px; border:2px solid purple; margin: auto; display: flex; flex-wrap: wrap; } div.resim { width: 300px; height: 300px; margin: 5px; img { width: 100%; height: 100%; border-radius: 100px 10px 100px 10px; } }
      </style>
  </head>
  <body>
    <h1><center>RESİM GALERİSİ</center></h1>
     <div id="kutuResim">
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
      <div class="resim"></div>
    </div>
    <script>
     const urlAl = 'https://source.unsplash.com/random/';
      var rasgelRes = new Array();
      for (let i = 0; i < 15; i++) {
        rasgelRes[i] = urlAl + boyut();
      }
      var resimgaleri = document.getElementsByClassName('resim');
      for (let a = 0; a < 15; a++) {
        resimgaleri[a].innerHTML =
          resimgaleri[a].innerHTML + '<img src=' + rasgelRes[a] + ' />';
        console.log(resimgaleri[a]);
      }
      function rasgelNum() {
        return Math.floor(Math.random() * 10) + 300;
      }
      function boyut() {
        return `${rasgelNum()}x${rasgelNum()}`;
      }
    </script>
  </body>
</html>
 

  </body>
</html>
g resim galerisi.html…]()