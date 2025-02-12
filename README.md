<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Website Pribadi</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #A35C7A;
            color: white;
            margin: 0;
            padding: 20px;
            text-align: center;
        }
        .container {
            background-color: #FFCCE1;
            padding: 50px;
            border-radius: 15px;
            box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.2);
            width: 80%;
            max-width: 500px;
            margin: auto;
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
    </style>
    <script>
        function showPage(pageId) {
            let pages = document.getElementsByClassName("page");
            for (let page of pages) {
                page.style.display = "none";
            }
            document.getElementById(pageId).style.display = "block";
        }
    </script>
</head>
<body>
    <!-- Halaman Utama -->
    <div class="container page" id="home">
        <h1>Welcome Raiders💫</h1>
        <h3>Enjoy your visit, hope you like it</h3>
        <img src="Welcome.jpg" alt="Welcome Image">
        <button onclick="showPage('biodata')">Next Page</button>
    </div>

    <!-- Halaman Biodata -->
    <div class="container page" id="biodata" style="display: none;">
        <h2>📜Informasi Pribadi</h2>
        <img src="Picture1.jpeg" width="250" alt="Foto Profil">
        <p><strong>🧑 Nama:</strong> Asma Lutfi</p>
        <p><strong>📍 Tempat & tanggal lahir:</strong> Siwalempu, 07 Mei 2005</p>
        <p><strong>🏡 Alamat:</strong> Jl. Lengaru, Palu Timur</p>
        <p><strong>🎮 Hobi:</strong> Gaming and Reading</p>
        <button onclick="showPage('pendidikan')">Next Page</button>
        <button onclick="showPage('home')">Halaman Utama</button>
    </div>

    <!-- Halaman Pendidikan -->
    <div class="container page" id="pendidikan" style="display: none;">
        <h2>🎓Pendidikan👩🏻‍🎓</h2>
        <img src="Universitas Tadulako.jpg" width="300" height="200" alt="Pendidikan">
        <p><strong>🏩 Universitas:</strong> Tadulako</p>
        <p><strong>🏢 Fakultas:</strong> Teknik</p>
        <p><strong>📚 Program Studi:</strong> S1 Sistem Informasi</p>
        <button onclick="showPage('biodata')">Kembali ke Halaman 2</button>
        <button onclick="showPage('home')">Halaman Utama</button>
    </div>
</body>
</html>
