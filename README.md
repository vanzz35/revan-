<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Revan Putra | Portofolio</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #facc15;
      --bg: #0f172a;
      --card: #1e293b;
      --text: #f1f5f9;
      --gray: #94a3b8;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: var(--bg);
      color: var(--text);
    }

    nav {
      position: sticky;
      top: 0;
      background-color: var(--bg);
      display: flex;
      justify-content: space-between;
      padding: 20px 10%;
      align-items: center;
      box-shadow: 0 2px 10px rgba(0,0,0,0.5);
      z-index: 1000;
    }

    nav h1 {
      font-size: 24px;
      color: var(--primary);
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
    }

    nav ul li a {
      text-decoration: none;
      color: var(--text);
      font-weight: 500;
      transition: 0.3s;
    }

    nav ul li a:hover {
      color: var(--primary);
    }

    .hero {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      padding: 80px 20px 100px;
    }

    .hero img {
      width: 160px;
      height: 160px;
      border-radius: 50%;
      border: 4px solid var(--primary);
      box-shadow: 0 0 20px var(--primary);
      margin-bottom: 20px;
    }

    .hero h2 {
      font-size: 38px;
      margin-bottom: 10px;
    }

    .typing {
      color: var(--gray);
      font-size: 18px;
      height: 24px;
      margin-bottom: 20px;
    }

    .btn {
      background-color: var(--primary);
      color: black;
      padding: 12px 30px;
      border-radius: 8px;
      font-weight: bold;
      border: none;
      cursor: pointer;
      margin-top: 15px;
      transition: 0.3s;
      text-decoration: none;
      display: inline-block;
    }

    .btn:hover {
      background-color: #eab308;
      transform: scale(1.05);
    }

    .section {
      padding: 60px 10%;
    }

    .section h2 {
      font-size: 32px;
      text-align: center;
      margin-bottom: 30px;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 25px;
    }

    .card {
      background-color: var(--card);
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 15px rgba(0,0,0,0.3);
    }

    footer {
      text-align: center;
      padding: 25px;
      background: var(--bg);
      font-size: 14px;
      color: var(--gray);
    }
  </style>
</head>
<body>

  <nav>
    <h1>Revan Putra</h1>
    <ul>
      <li><a href="#tentang">Tentang</a></li>
      <li><a href="#projek">Projek</a></li>
      <li><a href="#kontak">Kontak</a></li>
    </ul>
  </nav>

  <section class="hero">
    <img src="foto-revan-circular.png" alt="Foto Revan">
    <h2>Halo, Saya Revan 👋</h2>
    <div class="typing" id="typing"></div>
  </section>

  <section class="section" id="tentang">
    <h2>Tentang Saya</h2>
    <p style="text-align: center; max-width: 700px; margin: auto; color: var(--gray);">
      Saya pelajar SMK jurusan RPL yang suka membangun web interaktif dan estetis. Fokus saya adalah menggabungkan desain UI dengan pemrograman modern seperti HTML, CSS, dan JavaScript.
    </p>
  </section>

  <section class="section" id="projek">
    <h2>Proyek Terbaru</h2>
    <div class="grid">
      <div class="card">
        <h3>Landing Page Shopee</h3>
        <p>Clone halaman Shopee dengan daftar produk, dark mode, dan fitur pencarian.</p>
        <a href="shopee.html" class="btn">Lihat Proyek</a>
      </div>
      <div class="card">
        <h3>Form Login</h3>
        <p>Form login dengan validasi JavaScript dan desain modern.</p>
         <a href="login.html" class="btn">Lihat Proyek</a>
      </div>
      <div class="card">
        <h3>Aplikasi Desain Jersey</h3>
        <p>Desain jersey 3D dengan upload logo dan warna custom.</p>
      </div>
    </div>
  </section>

  <section class="section" id="kontak">
    <h2>Kontak Saya</h2>
    <div style="text-align: center;">
      <a href="mailto:revan@example.com" class="btn">Email</a>
      <a href="https://github.com/revanputra" class="btn">GitHub</a>
    </div>
  </section>

  <footer>
    &copy; 2025 Revan Putra. Dibuat dengan ❤️ + kopi.
  </footer>

  <script>
    const text = "Web Developer | UI Designer | Pelajar SMK";
    let i = 0;
    function typingEffect() {
      if (i < text.length) {
        document.getElementById("typing").textContent += text.charAt(i);
        i++;
        setTimeout(typingEffect, 50);
      }
    }
    typingEffect();
  </script>
</body>
</html>
