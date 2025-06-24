<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LBH-UIT Makassar</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" crossorigin="anonymous" />
  <style>
    :root {
      --bg-main: linear-gradient(135deg, #0f172a, #1e293b);
      --text-main: #e2e8f0;
      --highlight: #FFD700;
      --card-bg: rgba(255, 255, 255, 0.06);
    }
    .light-mode {
      --bg-main: linear-gradient(135deg, #fefefe, #e2e8f0);
      --text-main: #1e293b;
      --highlight: #0f172a;
      --card-bg: rgba(255, 255, 255, 0.6);
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: var(--bg-main);
      background-attachment: fixed;
      color: var(--text-main);
      transition: background 0.5s, color 0.5s;
    }
    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      color: var(--highlight);
    }
    .primary-color {
      background: var(--bg-main);
    }
    .text-highlight {
      color: var(--highlight);
    }
    .glass {
      background: var(--card-bg);
      border: 1px solid rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(20px);
      box-shadow: 0 8px 32px 0 rgba(255, 255, 255, 0.05);
      transition: background 0.5s;
    }
    .section {
      display: none;
      opacity: 0;
      transform: translateY(30px);
      transition: all 0.6s ease-in-out;
    }
    .section.active {
      display: block;
      opacity: 1;
      transform: translateY(0);
    }
    .hover-card {
      transition: transform 0.3s ease, background-color 0.3s ease;
    }
    .hover-card:hover {
      transform: scale(1.03);
      background-color: rgba(255, 255, 255, 0.08);
    }
    input, textarea {
      color: #0f172a;
    }
    a:hover {
      color: #00BFFF;
    }
    footer:hover {
      background: rgba(0, 0, 0, 0.1);
    }
  </style>
</head>
<body class="transition-all">
  <header class="primary-color text-white py-8 shadow-md text-center">
    <div class="flex flex-col items-center space-y-4">
      <img src="LOGO_LBH-removebg-preview.png" alt="Logo LBH-UIT" class="h-28 w-28 object-contain rounded-full border-4 border-white shadow-lg">
      <h1 class="text-4xl sm:text-5xl font-bold">LBH-UIT</h1>
      <p class="text-lg sm:text-xl text-center">Lembaga Bantuan Hukum<br>Universitas Indonesia Timur</p>
      <div class="flex flex-wrap justify-center gap-4 mt-4">
        <nav class="flex flex-wrap justify-center gap-6 text-lg font-semibold">
          <a href="#" onclick="showSection('beranda')" class="hover:text-yellow-300 transition">Beranda</a>
          <a href="#" onclick="showSection('tentang')" class="hover:text-yellow-300 transition">Tentang</a>
          <a href="#" onclick="showSection('layanan')" class="hover:text-yellow-300 transition">Layanan</a>
          <a href="#" onclick="showSection('struktur')" class="hover:text-yellow-300 transition">Struktur</a>
          <a href="#" onclick="showSection('dokumen')" class="hover:text-yellow-300 transition">Dokumen</a>
          <a href="#" onclick="showSection('kontak')" class="hover:text-yellow-300 transition">Kontak</a>
          <a href="#" onclick="showSection('pengaduan')" class="hover:text-yellow-300 transition">Pengaduan</a>
        </nav>
        <button onclick="toggleMode()" class="ml-4 px-4 py-1 bg-yellow-400 text-black rounded shadow hover:bg-yellow-500 transition">Toggle Tema</button>
      </div>
    </div>
  </header>

  <main class="px-6 py-16">
    <section id="beranda" class="section active text-center max-w-3xl mx-auto glass p-10 rounded-xl">
      <h2 class="text-4xl font-bold mb-4 lang" data-id="beranda-title">Mewujudkan Keadilan, Mengabdi untuk Masyarakat</h2>
      <p class="text-lg text-gray-300 lang" data-id="beranda-desc">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </section>
    <!-- Bagian lain tidak diubah -->
  </main>

  <footer class="primary-color text-white text-center py-6 transition-all">
    <p class="text-sm">&copy; 2025 LBH-UIT. Semua Hak Dilindungi.</p>
  </footer>

  <script>
    function showSection(id) {
      document.querySelectorAll('.section').forEach(section => section.classList.remove('active'));
      const target = document.getElementById(id);
      target.classList.add('active');
    }

    function toggleMode() {
      document.body.classList.toggle('light-mode');
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
