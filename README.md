<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pembelajaran Bulu Tangkis</title>
  <style>
    body {
      font-family: sans-serif;
      background: linear-gradient(to right, #87ceeb, #e0ffff); 
      margin: 0;
    }

    header {
      background-color: #333;
      color: #fff;
      padding: 20px; 
      text-align: center;
    }

    nav ul {
      list-style-type: none;
      margin: 0;
      padding: 0;
      background-color: #444;
      text-align: center;
    }

    nav ul li {
      display: inline;
      margin: 0 15px;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      padding: 10px;
      display: inline-block;
    }

    .search-container {
      margin-top: 10px;
    }

    .search-container input[type="text"] {
      padding: 8px;
      font-size: 16px;
      border-radius: 5px;
      border: 1px solid #ddd;
    }

    .search-container button {
      padding: 8px 15px;
      font-size: 16px;
      border: none;
      background-color: #444;
      color: #fff;
      border-radius: 5px;
      cursor: pointer;
    }

    .search-container button:hover {
      background-color: #666;
    }

    main {
      padding: 20px;
    }

    section {
      margin-bottom: 30px;
      background-color: #fff;
      padding: 20px;
      border-radius: 5px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
    }

    h2 {
      color: #333;
    }

    .teknik-gambar {
      float: left;
      margin-right: 20px;
      border: 1px solid #ddd;
      padding: 5px;
      border-radius: 5px;
    }

    footer {
      background-color: #333;
      color: #fff;
      text-align: center;
      padding: 10px;
      position: fixed;
      bottom: 0;
      width: 100%;
    }

    /* Efek marquee menggunakan CSS */
    .marquee {
      font-size: 24px;
      color: #333;
      white-space: nowrap;
      overflow: hidden;
      width: 100%;
      animation: marquee 10s linear infinite;
    }

    @keyframes marquee {
      0% {
        transform: translateX(100%);
      }
      100% {
        transform: translateX(-100%);
      }
    }
  </style>
</head>
<body>
  <!-- Teks berjalan -->
  <div class="marquee">Selamat datang di website pembelajaran bulu tangkis!</div>

  <header>
    <h1>Selamat Datang di Website Pembelajaran Bulu Tangkis</h1>
    <nav>
      <ul>
        <li><a href="#">Beranda</a></li>
        <li><a href="#">Teknik Dasar</a></li>
        <li><a href="#">Peraturan</a></li>
        <li><a href="#">Tips & Trik</a></li>
      </ul>
    </nav>

    <!-- Form Pencarian -->
    <div class="search-container">
      <input type="text" id="search" placeholder="Cari teknik bulu tangkis...">
      <button onclick="searchFunction()">Cari</button>
    </div>
  </header>

  <main>
    <section>
      <h2>Olahraga Bulu Tangkis</h2>
      <p>Bulu tangkis adalah olahraga raket yang dimainkan oleh dua pemain lawan (tunggal) atau dua pasangan lawan (ganda), yang menempati posisi berlawanan di setengah lapangan yang dibagi oleh net. Pemain mencetak poin dengan memukul kok dengan raket mereka sehingga melewati net dan jatuh di setengah lapangan lawan mereka.</p>
    </section>

    <section>
      <h2>Teknik Dasar</h2>
      <p>Berikut beberapa teknik dasar dalam bulu tangkis:</p>
      <h3>Memegang Raket</h3>
      <p>Ada dua cara memegang raket, yaitu forehand grip dan backhand grip.  Forehand grip digunakan untuk memukul kok yang datang dari sisi kanan badan, sedangkan backhand grip digunakan untuk memukul kok dari sisi kiri badan.</p>
      <h3>Servis</h3>
      <p>Servis adalah pukulan pertama untuk memulai permainan dalam bulu tangkis. Ada beberapa jenis servis, seperti servis pendek, servis panjang, dan flick serve.</p>
      <h3>Netting</h3>
      <p>Netting adalah teknik pukulan yang dilakukan di dekat net dengan tujuan agar kok jatuh di area depan lapangan lawan.</p>
      <h3>Overhead Clear</h3>
      <p>Overhead clear adalah pukulan yang dilakukan dari atas kepala dengan tujuan untuk menerbangkan kok ke bagian belakang lapangan lawan.</p>
      <h3>Drop Shot</h3>
      <p>Drop shot adalah pukulan yang bertujuan untuk menjatuhkan kok sedekat mungkin dengan net di lapangan lawan.</p>
      <h3>Smash</h3>
      <p>Smash adalah pukulan keras yang dilakukan dari atas kepala dengan tujuan untuk menghantam kok ke bawah di lapangan lawan.</p>
    </section>

    <section>
      <h2>Peraturan</h2>
      <p>Beberapa peraturan dasar dalam bulu tangkis:</p>
      <ul>
        <li>Permainan dimulai dengan servis dari area servis yang benar.</li>
        <li>Kok hanya boleh dipukul sekali di setiap sisi lapangan.</li>
        <li>Pemain kehilangan poin jika kok jatuh di luar lapangan atau menyentuh net.</li>
        <li>Permainan biasanya dimainkan hingga 21 poin.</li>
      </ul>
    </section>

    <section>
      <h2>Tips & Trik</h2>
      <p>Beberapa tips untuk bermain bulu tangkis dengan baik:</p>
      <ul>
        <li>Lakukan pemanasan sebelum bermain.</li>
        <li>Latih teknik dasar secara rutin.</li>
        <li>Perhatikan posisi kaki dan gerakan badan.</li>
        <li>Jaga fokus dan konsentrasi selama bermain.</li>
      </ul>
    </section>
  </main>

  <footer>
    <p>&copy; 2024 Website Pembelajaran Bulu Tangkis Ipan Irpandi 232223110</p>
  </footer>

  <script>
    function searchFunction() {
      let input = document.getElementById('search').value.toLowerCase();
      let sections = document.querySelectorAll('main section');
      
      sections.forEach(function(section) {
        let sectionText = section.textContent.toLowerCase();
        if (sectionText.includes(input)) {
          section.style.display = 'block';
        } else {
          section.style.display = 'none';
        }
      });
    }
  </script>

</body>
</html>

