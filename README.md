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
      background: linear-gradient(135deg, #0d1b2a, #1b263b); /* Biru gelap */
      background-attachment: fixed;
      color: #ffeb3b; /* Kuning */
    }
    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
      color: #ffeb3b;
    }
    .primary-color {
      background: linear-gradient(to right, #1b263b, #0d1b2a);
    }
    .text-highlight {
      color: #ffc107;
    }
    a, p, li, label {
      color: #ffeb3b;
    }
    a:hover {
      color: #ffd700;
    }
    input, textarea {
      color: #000;
      background-color: #fffde7;
    }
    .glass {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid rgba(255, 255, 255, 0.1);
      backdrop-filter: blur(16px);
      box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
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
      background-color: rgba(255, 255, 255, 0.1);
    }
    .text-gray-300 {
      color: #fff59d;
    }
    .glass p, .glass li {
      color: #fff176;
    }
    button {
      background-color: #ffc107;
      color: #000;
    }
    button:hover {
      background-color: #ffb300;
    }
    select {
      color: black;
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
      <h2 class="text-4xl font-bold mb-4 lang" data-id="beranda-title">Mewujudkan Keadilan, Mengabdi untuk Masyarakat</h2>
      <p class="text-lg text-gray-300 lang" data-id="beranda-desc">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </section>

    <section id="tentang" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-8 lang" data-id="visi">Visi</h2>
      <p class="text-gray-300 mb-10 leading-relaxed lang" data-id="visi-desc">Menjadi cahaya keadilan di tengah kabut ketimpangan, memperjuangkan hak setiap insan untuk hidup bermartabat dalam naungan hukum yang adil.</p>
      <h3 class="text-2xl font-semibold text-highlight mb-4 lang" data-id="misi">Misi</h3>
      <ol class="list-decimal text-left ml-6 space-y-4 text-lg text-gray-300">
        <li class="lang" data-id="misi-1">Menyediakan layanan bantuan hukum profesional bagi masyarakat miskin & rentan.</li>
        <li class="lang" data-id="misi-2">Mendorong reformasi hukum melalui advokasi & pendidikan.</li>
        <li class="lang" data-id="misi-3">Membangun sinergi nasional dan internasional untuk sistem hukum demokratis.</li>
        <li class="lang" data-id="misi-4">Menjunjung keadilan restoratif sebagai sarana pemulihan masyarakat.</li>
      </ol>
    </section>

    <section id="layanan" class="section max-w-5xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-10 lang" data-id="layanan-title">Jenis Pelayanan LBH-UIT</h2>
      <div class="grid sm:grid-cols-2 gap-6 text-left">
        <div class="p-4 rounded transition hover-card">
          <h3 class="text-xl font-semibold mb-2 lang" data-id="layanan-1-title">Bantuan Hukum</h3>
          <p class="lang" data-id="layanan-1-desc">Membantu masyarakat yang memerlukan bantuan hukum secara gratis.</p>
        </div>
        <div class="p-4 rounded transition hover-card">
          <h3 class="text-xl font-semibold mb-2 lang" data-id="layanan-2-title">Pendidikan Paralegal</h3>
          <p class="lang" data-id="layanan-2-desc">Menyediakan pendidikan dan pelatihan paralegal kepada masyarakat.</p>
        </div>
        <div class="p-4 rounded transition hover-card">
          <h3 class="text-xl font-semibold mb-2 lang" data-id="layanan-3-title">Pemantauan & Advokasi</h3>
          <p class="lang" data-id="layanan-3-desc">Melaporkan pelanggaran hukum oleh penegak hukum atau pemerintah.</p>
        </div>
        <div class="p-4 rounded transition hover-card">
          <h3 class="text-xl font-semibold mb-2 lang" data-id="layanan-4-title">Tempat Magang</h3>
          <p class="lang" data-id="layanan-4-desc">Menyediakan tempat magang untuk mahasiswa dan profesi hukum.</p>
        </div>
      </div>
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

    <section id="pengaduan" class="section max-w-3xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Form Pengaduan</h2>
      <form class="space-y-6 text-left text-gray-900">
        <div>
          <label class="block mb-1">Nama Lengkap</label>
          <input type="text" class="w-full p-2 rounded bg-white" placeholder="Nama Anda" />
        </div>
        <div>
          <label class="block mb-1">Email / No. HP</label>
          <input type="text" class="w-full p-2 rounded bg-white" placeholder="Kontak yang bisa dihubungi" />
        </div>
        <div>
          <label class="block mb-1">Isi Pengaduan</label>
          <textarea rows="4" class="w-full p-2 rounded bg-white" placeholder="Tulis pengaduan Anda..."></textarea>
        </div>
        <button type="submit" class="bg-green-600 text-white px-6 py-2 rounded hover:bg-green-700 transition">Kirim</button>
      </form>
    </section>

    <section id="kontak" class="section max-w-3xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
      <div class="text-lg text-gray-300 space-y-4">
        <p><i class="fab fa-whatsapp text-green-400 mr-2"></i> <a href="https://wa.me/6285299383003" class="text-green-400 underline">0852-9938-3003</a></p>
        <p><i class="fas fa-envelope text-red-300 mr-2"></i> <a href="mailto:lembagabantuanhukumit@gmail.com" class="text-blue-400 underline">lembagabantuanhukumit@gmail.com</a></p>
        <p><i class="fab fa-facebook text-blue-500 mr-2"></i> <a href="https://www.facebook.com/LembagaBantuanHukumUit" class="text-blue-300 underline">Lembaga Bantuan Hukum Uit</a></p>
        <p><i class="fab fa-instagram text-pink-500 mr-2"></i> <a href="https://www.instagram.com/lembaga_bantuan_hukum_uit" class="text-pink-300 underline">@lembaga_bantuan_hukum_uit</a></p>
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
