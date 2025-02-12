<html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Pribadi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #A35C7A;
            color: #A35C7A;
            margin: 0;
            padding: 0;
            text-align: center;
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        .container {
            background-color: #FFCCE1;
            padding: 80px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            width: 80%;
            max-width: 500px;
            display: none;
        }
        .active {
            display: block;
        }
        img {
            width: 250px;
            height: auto;
            border-radius: 10px;
            margin-bottom: 15px;
            border: 3px solid white;
            transition: transform 0.3s ease;
        }
        img:hover {
            transform: scale(1.1);
        }
        button {
            background-color: white;
            color: #A35C7A;
            border: none;
            padding: 10px 15px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: bold;
            display: block;
            margin: 20px auto;
        }
        button:hover {
            background-color: #f5f5f5;
        }
        h1, h2, h3, p, strong {
            color: #A35C7A;
        }
    </style>
</head>
<body>
    <div class="container active" id="page1">
        <h1>Welcome Raiders💫</h1>
        <h3>Enjoy your visit, hope you like it</h3>
        <img src="Welcome.jpg" alt="Welcome Image">
        <button onclick="window.location.href='Page2.html'">Next Page</button>
    </div>

    <div class="container" id="page2">
        <h2>📜Informasi Pribadi</h2>
        <img src="Picture 1.jpeg" width="300" height="500" alt="Foto Profil">
        <p><strong>🧑 Nama:</strong> Asma Lutfi</p>
        <p><strong>📍 Tempat & tanggal lahir:</strong> Siwalempu, 07 Mei 2005</p>
        <p><strong>🏡 Alamat:</strong> Jl. Lengaru, Palu Timur</p>
        <p><strong>🎮 Hobi:</strong> Gaming and Reading</p>
        <p><strong>🍦 Makanan Favorit:</strong> Es Krim</p>
        <p><strong>🥤 Minuman Favorit:</strong> Susu Strawberry</p>
        <p><strong>🎶 Musik Favorit:</strong> Blessing Cover by TNF</p>
        <button onclick="window.location.href='Page1.html'">Kembali</button>
        <button onclick="window.location.href='Page3.html'">Next Page</button>
    </div>

    <div class="container" id="page3">
        <h2>🎓Pendidikan👩🏻‍🎓</h2>
        <img src="Universitas Tadulako.jpg" width="300" height="200" alt="Pendidikan">
        <p><strong>🏩 Universitas:</strong> Tadulako</p>
        <p><strong>🏢 Fakultas:</strong> Teknik</p>
        <p><strong>📚 Program Studi:</strong> S1 Sistem Informasi</p>
        <button onclick="window.location.href='Page2.html'">Kembali</button>
        <button onclick="window.location.href='Page1.html'">Halaman Utama</button>
    </div>

    <script>
        function showPage(pageNumber) {
            document.querySelectorAll('.container').forEach(container => {
                container.classList.remove('active');
            });
            document.getElementById('page' + pageNumber).classList.add('active');
        }
    </script>
</body>
</html>
