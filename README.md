<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multi Page Biodata</title>
    <style>
        body {
            font-family: Little Summer, Arial, sans-serif;
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
            color: #A35C7A;
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
            document.querySelectorAll('.page').forEach(page => {
                page.style.display = 'none';
            });
            document.getElementById(pageId).style.display = 'block';
        }
    </script>
</head>
<body>
    <div class="container page" id="page1">
        <h1>Welcome Raiders💫</h1>
        <h3>Enjoy your visit, hope you like it</h3>
        <img src="Welcome.jpg" alt="Welcome Image">
        <button onclick="showPage('page2')">Next Page</button>
    </div>

    <div class="container page" id="page2" style="display:none;">
        <h2>📜Informasi Pribadi</h2>
        <img src="Picture 1.jpeg" alt="Foto Profil">
        <p><strong>🧑 Nama:</strong> Asma Lutfi</p>
        <p><strong>📍 Tempat & tanggal lahir:</strong> Siwalempu, 07 Mei 2005</p>
        <p><strong>🏡 Alamat:</strong> Jl. Lengaru, Palu Timur</p>
        <p><strong>🎮 Hobi:</strong> Gaming and Reading</p>
        <p><strong>🍦 Makanan Favorit:</strong> Es Krim</p>
        <p><strong>🥤 Minuman Favorit:</strong> Susu Strawberry</p>
        <p><strong>🎶 Musik Favorit:</strong> Blessing Cover by TNF</p>
        <button onclick="showPage('page3')">Next Page</button>
    </div>

    <div class="floating-gallery">
        <div class="image-container left">
            <img src="Picture 3.jpeg" alt="Foto 1">
            <p class="text">🌱Kesuksesan bukan tentang seberapa cepat kamu sampai, tapi seberapa konsisten kamu melangkah✨</p>
        </div>
        <div class="image-container right">
            <img src="Picture 6.jpeg" alt="Foto 2">
            <p class="text">🌟 "Jadilah perubahan yang ingin kamu lihat di dunia💖</p>
        </div>
    </div>

    <div class="container page" id="page3" style="display:none;">
        <h2>🎓Pendidikan👩🏻‍🎓</h2>
        <img src="Universitas Tadulako.jpg" width="300" height="200" alt="Pendidikan">
        <p><strong>🏩 Universitas:</strong> Tadulako</p>
        <p><strong>🏢 Fakultas:</strong> Teknik</p>
        <p><strong>📚 Program Studi:</strong> S1 Sistem Informasi</p>
        <button onclick="showPage('page1')">Halaman Utama</button>
        <button onclick="showPage('page2')">Kembali ke Halaman 2</button>
    </div>
</body>
</html>
