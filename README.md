<!-- ==========================
   Website LBH-UIT - Versi Profil Lengkap
   Menggunakan: Tailwind CSS, Glassmorphism, Navigasi Dinamis
   ========================== -->

<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Profil LBH-UIT</title>
  <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600&family=Poppins:wght@400;600&display=swap" rel="stylesheet" />
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
    .rounded-logo {
      border-radius: 50%;
      border: 4px solid white;
      box-shadow: 0 0 10px rgba(255, 255, 255, 0.2);
    }
  </style>
</head>
<body>
  <header class="primary-color text-white py-6 shadow-md text-center">
    <h1 class="text-4xl font-bold">LBH-UIT Makassar</h1>
    <nav class="mt-4 flex justify-center gap-6 text-lg font-semibold">
      <a href="#" onclick="showSection('profil')" class="hover:text-orange-300 transition">Profil</a>
      <a href="#" onclick="showSection('visi-misi')" class="hover:text-orange-300 transition">Visi Misi</a>
      <a href="#" onclick="showSection('struktur')" class="hover:text-orange-300 transition">Struktur</a>
      <a href="#" onclick="showSection('dokumen')" class="hover:text-orange-300 transition">Dokumen Legal</a>
      <a href="#" onclick="showSection('kontak')" class="hover:text-orange-300 transition">Kontak</a>
    </nav>
  </header>

  <main class="px-6 py-12">

    <!-- Profil -->
    <section id="profil" class="section active max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Profil LBH-UIT</h2>
      <img src="LOGO_LBH-removebg-preview.png" alt="Logo LBH-UIT" class="mx-auto h-32 mb-6 rounded-logo">
      <p class="text-gray-300 text-justify leading-loose">
        Lembaga Bantuan Hukum Universitas Indonesia Timur (LBH-UIT) merupakan perkumpulan berbadan hukum yang didirikan melalui Akta Notaris <strong>Mira Nila Kusuma Dewi, S.H., M.Kn.</strong> dengan nomor akta <strong>02 tanggal 12 Februari 2025</strong>. LBH-UIT telah disahkan oleh Menteri Hukum dan HAM Republik Indonesia melalui Keputusan Nomor <strong>AHU-0001101.AH.01.07.Tahun 2025</strong>.
      </p>
      <p class="text-gray-300 text-justify mt-4 leading-loose">
        Berkedudukan di <strong>Kota Makassar</strong> dan didaftarkan di <strong>Kabupaten Pangkajene dan Kepulauan</strong>, LBH-UIT hadir untuk memperjuangkan keadilan, mendampingi masyarakat marjinal, dan menyediakan layanan hukum berkualitas bagi masyarakat yang membutuhkan.
      </p>
    </section>

    <!-- Visi Misi -->
    <section id="visi-misi" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Visi & Misi LBH-UIT</h2>
      <h3 class="text-xl font-semibold text-orange-300 mb-2">Visi</h3>
      <p class="text-gray-300 leading-relaxed mb-6">
        Menjadi cahaya keadilan di tengah kabut ketimpangan, memperjuangkan hak setiap insan untuk hidup bermartabat dalam naungan hukum yang adil.
      </p>
      <h3 class="text-xl font-semibold text-orange-300 mb-2">Misi</h3>
      <ol class="list-decimal text-left text-gray-300 ml-6 space-y-2">
        <li>Menyediakan layanan bantuan hukum yang profesional, transparan, dan berpihak kepada masyarakat miskin, marjinal, dan kelompok rentan.</li>
        <li>Mendorong reformasi hukum yang berpihak pada keadilan sosial melalui advokasi dan pendidikan hukum.</li>
        <li>Membangun sinergi dengan lembaga nasional dan internasional dalam memperkuat sistem hukum yang demokratis dan akuntabel.</li>
        <li>Menjunjung tinggi prinsip keadilan restoratif sebagai upaya untuk menjadikan hukum sebagai sarana pemulihan dan pemberdayaan masyarakat.</li>
      </ol>
    </section>

    <!-- Struktur Organisasi -->
    <section id="struktur" class="section max-w-4xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Struktur Organisasi LBH-UIT</h2>
      <img src="Struktur Kelembagaan.jpg" alt="Struktur Organisasi LBH-UIT" class="rounded-lg shadow-lg mx-auto max-h-[500px]">
      <p class="text-gray-300 text-sm mt-4">Sumber: Lampiran SK Kemenkumham 2025</p>
    </section>

    <!-- Dokumen Legal -->
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

    <!-- Kontak Kami -->
    <section id="kontak" class="section max-w-3xl mx-auto glass p-10 rounded-xl text-center">
      <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
      <div class="text-lg text-gray-300 space-y-4">
        <p><i class="fas fa-envelope text-red-300 mr-2"></i> <a href="mailto:lembagabantuanhukumuit@gmail.com" class="text-blue-400 underline">lembagabantuanhukumuit@gmail.com</a></p>
        <p><i class="fab fa-whatsapp text-green-400 mr-2"></i> <a href="https://wa.me/6285299383003" class="text-green-400 underline">0852-9938-3003</a></p>
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
  </script>
</body>
</html>
