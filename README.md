<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Valentine untuk Kamu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #ffcccc;
            text-align: center;
            display: none;
        }
        .container {
            max-width: 600px;
            margin: 50px auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #ff4d6d;
        }
        .hidden {
            display: none;
        }
        #gallery img {
            width: 80%;
            margin: 10px;
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <div id="login-screen">
        <h1>Masukkan Sandi untuk Membuka Hadiah Valentine</h1>
        <input type="password" id="password" placeholder="Masukkan Sandi">
        <button onclick="checkPassword()">Buka</button>
        <p id="error-message" style="color: red; display: none;">Sandi salah! Coba lagi.</p>
    </div>

    <div id="content" class="hidden">
        <div class="container">
            <h1>Happy Valentine’s Day!</h1>
            <p>Untuk kamu yang spesial,</p>
            <p>Hari ini, aku ingin mengungkapkan betapa berartinya kamu dalam hidupku...</p>
            <p>(Tambahkan isi surat di sini)</p>
        </div>

        <div class="container">
            <h2>Galeri Foto Kita</h2>
            <div id="gallery">
                <img src="foto1.jpg" alt="Foto 1">
                <img src="foto2.jpg" alt="Foto 2">
                <img src="foto3.jpg" alt="Foto 3">
            </div>
        </div>
    </div>

    <script>
        function checkPassword() {
            var password = document.getElementById("password").value;
            if (password === "14 Februari 2025") {
                document.getElementById("login-screen").style.display = "none";
                document.getElementById("content").classList.remove("hidden");
                document.body.style.display = "block";
            } else {
                document.getElementById("error-message").style.display = "block";
            }
        }
    </script>

</body>
</html>
