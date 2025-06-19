<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LBH-UIT Makassar</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" crossorigin="anonymous" />
  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: url('02942530-ae4c-4f59-bfb6-870f5bbc903b.png') no-repeat center center fixed;
      background-size: cover;
      color: white;
    }
    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
    }
    .primary-color {
      background: #7a1c1c;
    }
    .text-highlight {
      color: #ffab91;
    }
    .glass {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(16px);
      box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.1);
    }
    .section {
      display: none;
      opacity: 0;
      transform: translateY(20px);
      transition: all 0.4s ease-in-out;
    }
    .section.active {
      display: block;
      opacity: 1;
      transform: translateY(0);
    }
    .hover-card:hover {
      transform: scale(1.03);
      background-color: rgba(255,255,255,0.1);
    }
    .text-gray-300 {
      color: #f0f0f0;
    }
    input, textarea {
      color: #000;
    }
    .glass p, .glass li {
      color: #f0f0f0;
    }
  </style>
</head>
<body>
  <header class="primary-color text-white py-8 shadow-md text-center">
    <div class="flex flex-col items-center space-y-4">
      <img src="LOGO_LBH-removebg-preview.png" alt="Logo LBH-UIT" class="h-28 w-28 object-contain rounded-full border-4 border-white shadow-lg">
      <h1 class="text-4xl sm:text-5xl font-bold">LBH-UIT</h1>
      <p class="text-lg sm:text-xl text-center">Lembaga Bantuan Hukum<br>Universitas Indonesia Timur</p>
      <div class="flex justify-between items-center gap-4 mt-4">
        <nav class="flex flex-wrap justify-center gap-6 text-lg font-semibold">
          <a href="#" onclick="showSection('beranda')" class="hover:text-orange-300 transition">Beranda</a>
          <a href="#" onclick="showSection('tentang')" class="hover:text-orange-300 transition">Tentang</a>
          <a href="#" onclick="showSection('layanan')" class="hover:text-orange-300 transition">Layanan</a>
          <a href="#" onclick="showSection('struktur')" class="hover:text-orange-300 transition">Struktur</a>
          <a href="#" onclick="showSection('dokumen')" class="hover:text-orange-300 transition">Dokumen Legal</a>
          <a href="#" onclick="showSection('kontak')" class="hover:text-orange-300 transition">Kontak</a>
          <a href="#" onclick="showSection('pengaduan')" class="hover:text-orange-300 transition">Pengaduan</a>
        </nav>
        <select onchange="changeLanguage(this.value)" class="ml-4 px-2 py-1 bg-white text-black rounded">
          <option value="id">ID</option>
          <option value="en">EN</option>
        </select>
      </div>
    </div>
  </header>

  <main class="px-6 py-16">
    <section id="beranda" class="section active text-center max-w-3xl mx-auto glass p-10 rounded-xl">
      <h2 class="text-4xl font-bold mb-4 lang" data-id="beranda-title">Mewujudkan Keadilan Mengabdi untuk Masyarakat</h2>
      <p class="text-lg text-gray-300 lang" data-id="beranda-desc">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </section>

    <section id="struktur" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Struktur Organisasi LBH-UIT</h2>
      <img src="Struktur Kelembagaan.jpg" alt="Struktur Organisasi" class="rounded-lg shadow-lg mx-auto max-h-[500px]">
      <p class="text-sm mt-4 text-gray-300">Sumber: Lampiran SK Kemenkumham 2025</p>
    </section>

    <section id="dokumen" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Dokumen Legalitas</h2>
      <div class="grid md:grid-cols-2 gap-6">
        <div>
          <h3 class="text-lg text-orange-300 font-semibold mb-2">Akta Pendirian</h3>
          <img src="Akta Pendirian.jpg" alt="Akta Pendirian" class="rounded shadow-md mx-auto">
        </div>
        <div>
          <h3 class="text-lg text-orange-300 font-semibold mb-2">SK Kemenkumham</h3>
          <img src="SK Kemenkumham.jpg" alt="SK Kemenkumham" class="rounded shadow-md mx-auto">
        </div>
      </div>
    </section>
  </main>

  <footer class="primary-color text-white text-center py-6">
    <p class="text-sm">&copy; 2025 LBH-UIT. Semua Hak Dilindungi.</p>
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll('.section').forEach(section => section.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }

    const translations = {
      en: {
        "beranda-title": "Fighting for Justice and Serving the People",
        "beranda-desc": "LBH-UIT is here to assist the public in need of justice and legal protection."
      }
    };

    function changeLanguage(lang) {
      document.querySelectorAll('.lang').forEach(el => {
        const key = el.getAttribute('data-id');
        if (lang === 'en' && translations.en[key]) {
          el.textContent = translations.en[key];
        } else {
          location.reload();
        }
      });
    }
  </script>
</body>
</html>
