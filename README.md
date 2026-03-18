<!DOCTYPE html>
<html>
<head>
  <title>Lemari Kodenya [Nama Kamu]</title>
  <style>
    body { font-family: sans-serif; text-align: center; transition: 0.5s; padding: 50px; }
    .box { border: 2px solid #ddd; padding: 20px; margin: 20px auto; max-width: 400px; border-radius: 15px; }
    button { cursor: pointer; padding: 10px; border-radius: 5px; border: none; background: #3498db; color: white; }
    .foto-saya { width: 150px; transition: 0.3s; border-radius: 50%; margin-top: 10px; }
    .foto-saya:hover { transform: scale(1.2); }
  </style>
</head>
<body>

  <h1>Selamat Datang di Lemari Kode Saya! 📦</h1>
  
  <div class="box">
    <p>Laci 1: Kendali Cahaya</p>
    <button onclick="ubahWarna()">Klik Dark Mode</button>
  </div>

  <div class="box">
    <p>Laci 2: Kenalan Dong</p>
    <input type="text" id="inputNama" placeholder="Nama kamu...">
    <button onclick="sapaUser()">Sapa Saya</button>
    <h3 id="hasilSapaan"></h3>
  </div>

  <div class="box">
    <p>Laci 3: Foto Ajaib (Sentuh Saya)</p>
    <img src="https://via.placeholder.com/150" class="foto-saya">
  </div>

  <script>
    function ubahWarna() {
      if (document.body.style.backgroundColor === "black") {
        document.body.style.backgroundColor = "white";
        document.body.style.color = "black";
      } else {
        document.body.style.backgroundColor = "black";
        document.body.style.color = "white";
      }
    }

    function sapaUser() {
      let nama = document.getElementById("inputNama").value;
      document.getElementById("hasilSapaan").innerText = "Halo " + nama + ", senang belajar bareng kamu!";
    }
  </script>

</body>
</html>
