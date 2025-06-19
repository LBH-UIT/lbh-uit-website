<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>LBH-UIT Makassar</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Orbitron:wght@500;700&display=swap" rel="stylesheet" />
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css" integrity="sha512-RRyjghIO6mSMRzR8ZtZ8vjykEtdTVEPZAv/IYJkoX+7F/d6eVtT0jMiUWUctiY6RuMIyoA+V/4Y7svF1Obl2Og==" crossorigin="anonymous" referrerpolicy="no-referrer" />
  <style>
    body {
      font-family: 'Inter', sans-serif;
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
    .hero-gradient {
      background: linear-gradient(120deg, #144d36, #7a1c1c);
    }
    .hover-glow:hover {
      box-shadow: 0 0 20px rgba(255, 61, 0, 0.5);
      transform: translateY(-2px);
      transition: 0.3s ease-in-out;
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
          <h1 class="text-2xl sm:text-3xl font-bold leading-tight">LBH-UIT</h1>
          <p class="text-sm sm:text-base">Lembaga Bantuan Hukum<br>Universitas Indonesia Timur</p>
        </div>
      </div>
      <nav class="hidden sm:flex space-x-6 text-lg font-medium">
        <a href="#beranda" title="Informasi umum website" class="hover:text-orange-300 transition">Beranda</a>
        <a href="#tentang" title="Visi dan Misi LBH-UIT" class="hover:text-orange-300 transition">Tentang</a>
        <a href="#layanan" title="Pelayanan yang diberikan LBH-UIT" class="hover:text-orange-300 transition">Layanan</a>
        <a href="#kontak" title="Email, WhatsApp, Facebook & Instagram" class="hover:text-orange-300 transition">Kontak</a>
      </nav>
    </div>
  </header>

  <!-- Beranda -->
  <section id="beranda" class="hero-gradient text-white py-36 px-6">
    <div class="glass p-10 rounded-xl max-w-3xl mx-auto text-center">
      <h2 class="text-5xl font-bold mb-4">Mewujudkan Keadilan, Mengabdi untuk Rakyat</h2>
      <p class="text-lg text-gray-300">LBH-UIT hadir untuk membantu masyarakat yang membutuhkan keadilan dan perlindungan hukum.</p>
    </div>
  </section>

  <!-- Tentang -->
  <section id="tentang" class="py-20 px-6">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-4xl font-bold text-highlight mb-8">Tentang LBH-UIT</h2>

      <h3 class="text-2xl font-semibold text-highlight mb-4">Visi</h3>
      <p class="mb-10 text-lg text-gray-300 leading-relaxed">
        Menjadi cahaya keadilan di tengah kabut ketimpangan, memperjuangkan hak setiap insan untuk hidup bermartabat dalam naungan hukum yang adil.
      </p>

      <h3 class="text-2xl font-semibold text-highlight mb-4">Misi</h3>
      <ol class="list-decimal text-left ml-6 space-y-4 text-lg text-gray-300">
        <li>Menyediakan layanan bantuan hukum profesional bagi masyarakat miskin & rentan.</li>
        <li>Mendorong reformasi hukum melalui advokasi & pendidikan.</li>
        <li>Membangun sinergi nasional dan internasional untuk sistem hukum demokratis.</li>
        <li>Menjunjung keadilan restoratif sebagai sarana pemulihan masyarakat.</li>
      </ol>
    </div>
  </section>

  <!-- Layanan -->
  <section id="layanan" class="py-20 px-6">
    <div class="max-w-5xl mx-auto text-center">
      <h2 class="text-3xl font-bold text-highlight mb-10">Pelayanan LBH-UIT</h2>
      <div class="grid sm:grid-cols-2 gap-8 text-left">
        <div class="glass p-6 rounded-2xl hover-glow">
          <h3 class="text-xl font-semibold mb-2">Bantuan Hukum</h3>
          <p>Membantu masyarakat yang memerlukan bantuan hukum secara gratis.</p>
        </div>
        <div class="glass p-6 rounded-2xl hover-glow">
          <h3 class="text-xl font-semibold mb-2">Pendidikan Paralegal</h3>
          <p>Menyediakan pendidikan dan pelatihan paralegal kepada masyarakat.</p>
        </div>
        <div class="glass p-6 rounded-2xl hover-glow">
          <h3 class="text-xl font-semibold mb-2">Pemantauan & Advokasi</h3>
          <p>Melaporkan pelanggaran hukum oleh penegak hukum atau pemerintah.</p>
        </div>
        <div class="glass p-6 rounded-2xl hover-glow">
          <h3 class="text-xl font-semibold mb-2">Tempat Magang</h3>
          <p>Menyediakan tempat magang untuk mahasiswa dan profesi hukum.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Kontak -->
  <section id="kontak" class="py-20 px-6">
    <div class="max-w-4xl mx-auto text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
      <div class="space-y-4 text-lg text-gray-300">
        <p>Email: <a href="mailto:lbhuit501@gmail.com" class="text-blue-400 underline">lbhuit501@gmail.com</a></p>
        <p>WhatsApp: <a href="https://wa.me/6285299383003" class="text-green-400 underline">0852-9938-3003</a></p>
        <p>
          <i class="fab fa-facebook text-blue-500 mr-2"></i>
          Facebook: <a href="https://www.facebook.com/LembagaBantuanHukumUit" class="underline text-blue-300">Lembaga Bantuan Hukum Uit</a>
        </p>
        <p>
          <i class="fab fa-instagram text-pink-500 mr-2"></i>
          Instagram: <a href="https://www.instagram.com/lembaga_bantuan_hukum_uit" class="underline text-pink-300">@lembaga_bantuan_hukum_uit</a>
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
