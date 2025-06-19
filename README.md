<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LBH-UIT Makassar</title>

  <!-- Tailwind CSS -->
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
  
  <!-- Google Font: Poppins -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">

  <!-- Font Awesome (for social media icons) -->
  <script src="https://kit.fontawesome.com/a2d9a64db9.js" crossorigin="anonymous"></script>

  <style>
    body { font-family: 'Poppins', sans-serif; scroll-behavior: smooth; }
    .primary-color { background-color: #7a1c1c; }
    .text-highlight { color: #7a1c1c; }
    .glass {
      background: rgba(255, 255, 255, 0.2);
      backdrop-filter: blur(10px);
      box-shadow: 0 8px 32px 0 rgba(31, 38, 135, 0.37);
    }
    .hero-gradient {
      background: linear-gradient(135deg, #7a1c1c 0%, #000000 100%);
    }
    .nav-link:hover {
      color: #ffd8d8;
      transition: 0.3s;
    }
    .fade-in {
      animation: fadeIn 1s ease-in-out;
    }
    @keyframes fadeIn {
      0% { opacity: 0; transform: translateY(20px); }
      100% { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body class="bg-white text-gray-800">

  <!-- Header -->
  <header class="primary-color text-white py-6 shadow-lg sticky top-0 z-50">
    <div class="max-w-6xl mx-auto px-6 flex items-center justify-between">
      <div class="flex items-center space-x-4">
        <img src="LOGO_LBH-removebg-preview.png" alt="Logo LBH-UIT" class="h-14 w-14 object-contain rounded-full shadow-md">
        <div>
          <h1 class="text-2xl sm:text-3xl font-bold leading-tight tracking-wide">Lembaga Bantuan Hukum<br>
            <span class="text-sm sm:text-base font-medium">Universitas Indonesia Timur (LBH-UIT)</span>
          </h1>
        </div>
      </div>
      <nav class="hidden sm:flex space-x-6 text-lg font-medium">
        <a href="#beranda" class="nav-link">Beranda</a>
        <a href="#tentang" class="nav-link">Tentang Kami</a>
        <a href="#layanan" class="nav-link">Layanan</a>
        <a href="#kontak" class="nav-link">Kontak</a>
      </nav>
    </div>
  </header>

  <!-- Hero -->
  <section id="beranda" class="hero-gradient text-white py-32 px-6">
    <div class="glass p-10 rounded-xl max-w-3xl mx-auto text-center fade-in">
      <h2 class="text-5xl font-bold mb-4 leading-snug">Mewujudkan Keadilan, Mengabdi untuk Rakyat</h2>
      <p class="text-lg">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </div>
  </section>

  <!-- Tentang Kami -->
  <section id="tentang" class="py-20 bg-gray-100 px-6">
    <div class="max-w-5xl mx-auto text-center fade-in">
      <h2 class="text-3xl font-bold text-highlight mb-10">Tentang Kami</h2>
      <div class="text-left space-y-8">
        <!-- Visi -->
        <div>
          <h3 class="text-2xl font-semibold text-highlight mb-2">🎯 Visi</h3>
          <p class="text-lg leading-relaxed">Memperjuangkan hak setiap insan untuk hidup bermartabat dalam naungan hukum yang adil.</p>
        </div>

        <!-- Misi -->
        <div>
          <h3 class="text-2xl font-semibold text-highlight mb-2">📌 Misi</h3>
          <ol class="list-decimal ml-6 space-y-3 text-lg">
            <li>Memberikan layanan bantuan hukum yang profesional dan berpihak</li>
            <li>Mendorong reformasi hukum yang adil dan inklusif</li>
            <li>Membangun sinergi nasional dan internasional</li>
            <li>Menjunjung tinggi keadilan restoratif</li>
          </ol>
        </div>
      </div>
    </div>
  </section>

  <!-- Layanan -->
  <section id="layanan" class="py-20 bg-white px-6">
    <div class="max-w-5xl mx-auto text-center fade-in">
      <h2 class="text-3xl font-bold text-highlight mb-10">Pelayanan LBH-UIT</h2>
      <div class="grid sm:grid-cols-2 gap-8 text-left">
        <div class="bg-white border border-gray-200 p-6 rounded-2xl shadow hover:scale-105 transition duration-300">
          <h3 class="text-xl font-semibold mb-2 text-highlight">Bantuan Hukum</h3>
          <p>Membantu masyarakat yang memerlukan bantuan hukum secara gratis.</p>
        </div>
        <div class="bg-white border border-gray-200 p-6 rounded-2xl shadow hover:scale-105 transition duration-300">
          <h3 class="text-xl font-semibold mb-2 text-highlight">Pendidikan Paralegal</h3>
          <p>Menyediakan pendidikan dan pelatihan paralegal kepada masyarakat.</p>
        </div>
        <div class="bg-white border border-gray-200 p-6 rounded-2xl shadow hover:scale-105 transition duration-300">
          <h3 class="text-xl font-semibold mb-2 text-highlight">Pemantauan & Advokasi</h3>
          <p>Melaporkan pelanggaran hukum oleh penegak hukum atau pemerintah.</p>
        </div>
        <div class="bg-white border border-gray-200 p-6 rounded-2xl shadow hover:scale-105 transition duration-300">
          <h3 class="text-xl font-semibold mb-2 text-highlight">Tempat Magang</h3>
          <p>Menyediakan tempat magang untuk mahasiswa dan profesi hukum.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Kontak -->
  <section id="kontak" class="py-20 bg-gray-100 px-6">
    <div class="max-w-4xl mx-auto text-center fade-in">
      <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
      <div class="space-y-4 text-lg">
        <p><i class="fas fa-envelope text-red-700 mr-2"></i>Email: 
          <a href="mailto:lbhuit501@gmail.com" class="text-blue-600 underline">lbhuit501@gmail.com</a>
        </p>
        <p><i class="fab fa-whatsapp text-green-600 mr-2"></i>WhatsApp: 
          <a href="https://wa.me/6285299383003" class="text-green-600 underline">0852-9938-3003</a>
        </p>
        <p><i class="fab fa-facebook-square text-blue-700 mr-2"></i>Facebook: 
          <a href="https://www.facebook.com/LembagaBantuanHukumUit" class="text-blue-600 underline">Lembaga Bantuan Hukum Uit</a>
        </p>
        <p><i class="fab fa-instagram text-pink-500 mr-2"></i>Instagram: 
          <a href="https://www.instagram.com/lembaga_bantuan_hukum_uit" class="text-pink-600 underline">@lembaga_bantuan_hukum_uit</a>
        </p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="primary-color text-white text-center py-6 mt-12">
    <p class="text-sm">&copy; 2025 LBH-UIT. Semua Hak Dilindungi.</p>
  </footer>

</body>
</html>
