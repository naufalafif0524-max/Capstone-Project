<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Negeri Diatas Awan Citorek</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #f0f8ff;
      color: #333;
    }
    header {
      background: #2c3e50;
      color: white;
      padding: 1rem 2rem;
      text-align: center;
    }
    nav {
      background: #34495e;
      display: flex;
      justify-content: center;
      gap: 1rem;
    }
    nav button {
      background: none;
      border: none;
      color: white;
      padding: 1rem 1.5rem;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }
    nav button:hover, nav button.active {
      background: #1abc9c;
      color: #fff;
      border-radius: 4px;
    }
    main {
      padding: 2rem;
      max-width: 900px;
      margin: auto;
      min-height: 70vh;
      background: white;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 8px;
    }
    h1, h2 {
      color: #16a085;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #2c3e50;
      color: white;
      margin-top: 2rem;
    }
    iframe {
      width: 100%;
      height: 300px;
      border: none;
      border-radius: 8px;
    }
    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 500px;
      margin: auto;
    }
    label {
      font-weight: bold;
    }
    input, textarea, select {
      padding: 0.5rem;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 4px;
      resize: vertical;
    }
    .btn-submit {
      background: #16a085;
      color: white;
      border: none;
      padding: 0.75rem;
      cursor: pointer;
      font-size: 1rem;
      border-radius: 4px;
      transition: background 0.3s;
    }
    .btn-submit:hover {
      background: #13856e;
    }
    /* Responsive */
    @media (max-width: 600px) {
      nav {
        flex-direction: column;
        gap: 0.5rem;
      }
      main {
        padding: 1rem;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>Negeri Diatas Awan Citorek</h1>
  <p>Wisata Alam yang Menyentuh Langit</p>
</header>

<nav>
  <button class="nav-btn active" data-page="home">Beranda</button>
  <button class="nav-btn" data-page="about">Tentang</button>
  <button class="nav-btn" data-page="wisata">Wisata</button>
  <button class="nav-btn" data-page="produk">Produk & Kegiatan</button>
  <button class="nav-btn" data-page="contact">Kontak</button>
</nav>

<main id="content">
  <!-- Konten halaman akan dimuat di sini -->
</main>

<footer>
  &copy; 2024 Negeri Diatas Awan Citorek - Semua Hak Cipta Dilindungi
</footer>

<script>
  const pages = {
    home: `
      <h2>Selamat Datang di Negeri Diatas Awan Citorek</h2>
      <p>Temukan keindahan alam yang memukau, udara segar, dan pemandangan yang menakjubkan di Citorek, sebuah desa yang terletak di atas awan. Jelajahi situs ini untuk mengetahui lebih banyak tentang wisata, produk lokal, dan kegiatan menarik di sini.</p>
      <p><strong>Ayo mulai petualanganmu sekarang!</strong></p>
      <iframe width="560" height="315" src="https://www.youtube.com/embed/zH6QiBoD2-I?si=WO_ZyxU2-wtL75S-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
    `,
    about: `
      <h2>Tentang Negeri Diatas Awan Citorek</h2>
      <p>Citorek adalah sebuah desa yang terkenal dengan keindahan alamnya yang berada di ketinggian, seringkali diselimuti oleh awan yang menambah kesan magis. Komunitas di sini sangat ramah dan menjaga kelestarian lingkungan serta budaya lokal.</p>
      <p>Usaha lokal yang berkembang di Citorek meliputi kerajinan tangan, pertanian organik, dan wisata alam yang berkelanjutan.</p>
      <img src="Negri di atas awan" alt="Pemandangan Citorek" style="width:100%; border-radius:8px; margin-top:1rem;">
    `,
    wisata: `
      <h2>Wisata Alam di Citorek</h2>
      <p>Beberapa destinasi wisata yang wajib dikunjungi:</p>
      <ul>
        <li>Gunung Luhur - Pendakian dengan pemandangan spektakuler</li>
        <li>Curug Citorek - Air terjun alami yang menyejukkan</li>
        <li>Perkebunan Teh - Nikmati udara segar dan panorama hijau</li>
      </ul>
      <h3>Peta Lokasi Wisata</h3>
      <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3956.123456789012!2d106.123456789!3d-6.123456789!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e6a123456789abc%3A0x123456789abcdef!2sCitorek%2C%20Lebak%20Regency!5e0!3m2!1sen!2sid!4v1680000000000!5m2!1sen!2sid" allowfullscreen="" loading="lazy"></iframe>
    `,
    produk: `
      <h2>Produk Lokal dan Kegiatan</h2>
      <p>Citorek juga dikenal dengan produk lokal berkualitas dan berbagai kegiatan menarik:</p>
      <ul>
        <li>Kerajinan anyaman bambu dan rotan</li>
        <li>Produk pertanian organik seperti kopi dan sayur-sayuran</li>
        <li>Workshop budaya dan seni tradisional</li>
      </ul>
      <h3>Kalender Kegiatan</h3>
      <iframe src="https://calendar.google.com/calendar/embed?src=your_calendar_id%40group.calendar.google.com&ctz=Asia%2FJakarta" style="border: 0" width="100%" height="300" frameborder="0" scrolling="no"></iframe>
      <p><em>Ganti "your_calendar_id" dengan ID kalender Google Anda untuk menampilkan kalender kegiatan.</em></p>
    `,
    contact: `
      <h2>Kontak Kami</h2>
      <p>Untuk pertanyaan atau informasi lebih lanjut, silakan hubungi kami melalui formulir di bawah ini:</p>
      <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSfDUMMY_FORM_ID/viewform?embedded=true" width="100%" height="600" frameborder="0" marginheight="0" marginwidth="0">Memuat…</iframe>
      <p>Atau kunjungi langsung:</p>
      <ul>
        <li>Alamat: Desa Citorek, Kabupaten Lebak, Banten</li>
        <li>Email: info@citorek.com</li>
        <li>Telepon: +62 812 3456 7890</li>
      </ul>
    `
  };

  const contentDiv = document.getElementById('content');
  const navButtons = document.querySelectorAll('.nav-btn');

  function setActivePage(page) {
    contentDiv.innerHTML = pages[page];
    navButtons.forEach(btn => {
      btn.classList.toggle('active', btn.dataset.page === page);
    });
  }

  navButtons.forEach(btn => {
    btn.addEventListener('click', () => {
      setActivePage(btn.dataset.page);
    });
  });

  // Muat halaman home secara default
  setActivePage('home');
</script>

</body>
</html>
