<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LBH-UIT Makassar</title>

  <!-- Tailwind CSS -->
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@400;600&display=swap" rel="stylesheet" />

  <!-- Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" crossorigin="anonymous" />

  <style>
    body {
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(135deg, #144d36, #7a1c1c);
      background-attachment: fixed;
      color: white;
    }
    h1, h2, h3 {
      font-family: 'Orbitron', sans-serif;
    }
    .primary-color {
      background: linear-gradient(to right, #7a1c1c, #144d36);
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
    }
    .section.active {
      display: block;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header class="primary-color text-white py-5 sticky top-0 z-50 shadow-md">
    <div class="max-w-6xl mx-auto px-6 flex items-center justify-between">
      <div class="flex items-center space-x-4">
        <img src="LOGO_LBH-removebg-preview.png" alt="Logo LBH-UIT" class="h-14 w-14 object-contain rounded-full border-2 border-white shadow-md">
        <div>
          <h1 class="text-2xl sm:text-3xl font-bold">LBH-UIT</h1>
          <p class="text-sm">Lembaga Bantuan Hukum<br>Universitas Indonesia Timur</p>
        </div>
      </div>
      <nav class="hidden sm:flex space-x-6 text-lg font-medium">
        <a href="#" onclick="showSection('beranda')" class="hover:text-orange-300 transition">Beranda</a>
        <a href="#" onclick="showSection('tentang')" class="hover:text-orange-300 transition">Tentang</a>
        <a href="#" onclick="showSection('layanan')" class="hover:text-orange-300 transition">Layanan</a>
        <a href="#" onclick="showSection('kontak')" class="hover:text-orange-300 transition">Kontak</a>
      </nav>
    </div>
  </header>

  <!-- Main Content -->
  <main class="px-6 py-16">
    <!-- Beranda -->
    <section id="beranda" class="section active text-center max-w-3xl mx-auto glass p-10 rounded-xl">
      <h2 class="text-4xl font-bold mb-4">Mewujudkan Keadilan, Mengabdi untuk Rakyat</h2>
      <p class="text-lg text-gray-300">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </section>

    <!-- Tentang -->
    <section id="tentang" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-8">Visi</h2>
      <p class="text-gray-300 mb-10 leading-relaxed">
        Menjadi cahaya keadilan di tengah kabut ketimpangan, memperjuangkan hak setiap insan untuk hidup bermartabat dalam naungan hukum yang adil.
      </p>
      <h3 class="text-2xl font-semibold text-highlight mb-4">Misi</h3>
      <ol class="list-decimal text-left ml-6 space-y-4 text-lg text-gray-300">
        <li>Menyediakan layanan bantuan hukum profesional bagi masyarakat miskin & rentan.</li>
        <li>Mendorong reformasi hukum melalui advokasi & pendidikan.</li>
        <li>Membangun sinergi nasional dan internasional untuk sistem hukum demokratis.</li>
        <li>Menjunjung keadilan restoratif sebagai sarana pemulihan masyarakat.</li>
      </ol>
    </section>

    <!-- Layanan -->
    <section id="layanan" class="section max-w-5xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-10">Jenis Pelayanan LBH-UIT</h2>
      <div class="grid sm:grid-cols-2 gap-6 text-left">
        <div class="p-4 hover:bg-white hover:bg-opacity-10 rounded transition">
          <h3 class="text-xl font-semibold mb-2">Bantuan Hukum</h3>
          <p>Membantu masyarakat yang memerlukan bantuan hukum secara gratis.</p>
        </div>
        <div class="p-4 hover:bg-white hover:bg-opacity-10 rounded transition">
          <h3 class="text-xl font-semibold mb-2">Pendidikan Paralegal</h3>
          <p>Menyediakan pendidikan dan pelatihan paralegal kepada masyarakat.</p>
        </div>
        <div class="p-4 hover:bg-white hover:bg-opacity-10 rounded transition">
          <h3 class="text-xl font-semibold mb-2">Pemantauan & Advokasi</h3>
          <p>Melaporkan pelanggaran hukum oleh penegak hukum atau pemerintah.</p>
        </div>
        <div class="p-4 hover:bg-white hover:bg-opacity-10 rounded transition">
          <h3 class="text-xl font-semibold mb-2">Tempat Magang</h3>
          <p>Menyediakan tempat magang untuk mahasiswa dan profesi hukum.</p>
        </div>
      </div>
    </section>

    <!-- Kontak -->
    <section id="kontak" class="section max-w-3xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
      <div class="text-lg text-gray-300 space-y-4">
        <p>
          <i class="fas fa-envelope text-red-300 mr-2"></i>
          Email: <a href="mailto:lbhuit501@gmail.com" class="text-blue-400 underline">lbhuit501@gmail.com</a>
        </p>
        <p>
          <i class="fab fa-whatsapp text-green-400 mr-2"></i>
          WhatsApp: <a href="https://wa.me/6285299383003" class="text-green-400 underline">0852-9938-3003</a>
        </p>
        <p>
          <i class="fab fa-facebook text-blue-500 mr-2"></i>
          Facebook: <a href="https://www.facebook.com/LembagaBantuanHukumUit" class="text-blue-300 underline">Lembaga Bantuan Hukum Uit</a>
        </p>
        <p>
          <i class="fab fa-instagram text-pink-500 mr-2"></i>
          Instagram: <a href="https://www.instagram.com/lembaga_bantuan_hukum_uit" class="text-pink-300 underline">@lembaga_bantuan_hukum_uit</a>
        </p>
      </div>
    </section>
  </main>

  <!-- Footer -->
  <footer class="primary-color text-white text-center py-6">
    <p class="text-sm">&copy; 2025 LBH-UIT. Semua Hak Dilindungi.</p>
  </footer>

  <!-- Script -->
  <script>
    function showSection(id) {
      const sections = document.querySelectorAll('.section');
      sections.forEach(section => section.classList.remove('active'));
      document.getElementById(id).classList.add('active');
    }
  </script>

</body>
</html>
