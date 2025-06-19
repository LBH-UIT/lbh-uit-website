<!-- Modal Layanan -->
<div id="modalLayanan" class="modal fixed inset-0 bg-black bg-opacity-60 justify-center items-center z-50">
  <div class="bg-white rounded-xl max-w-3xl w-full p-8 relative fade-in">
    <button class="absolute top-4 right-4 text-red-600 text-xl font-bold" onclick="closeLayanan()">&times;</button>
    <h2 class="text-3xl font-bold text-highlight mb-6 text-center">Pelayanan LBH-UIT</h2>
    <div class="grid sm:grid-cols-2 gap-6 text-left">
      <div>
        <h3 class="text-xl font-semibold text-highlight mb-2">Bantuan Hukum</h3>
        <p class="text-gray-700">Membantu masyarakat yang memerlukan bantuan hukum secara gratis.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold text-highlight mb-2">Pendidikan Paralegal</h3>
        <p class="text-gray-700">Menyediakan pendidikan dan pelatihan paralegal kepada masyarakat.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold text-highlight mb-2">Pemantauan & Advokasi</h3>
        <p class="text-gray-700">Melaporkan pelanggaran hukum oleh penegak hukum atau pemerintah.</p>
      </div>
      <div>
        <h3 class="text-xl font-semibold text-highlight mb-2">Tempat Magang</h3>
        <p class="text-gray-700">Menyediakan tempat magang untuk mahasiswa dan profesi hukum.</p>
      </div>
    </div>
  </div>
</div>

<script>
  function openLayanan() {
    document.getElementById('modalLayanan').classList.add('active');
  }
  function closeLayanan() {
    document.getElementById('modalLayanan').classList.remove('active');
  }
</script>

<!-- Ubah tautan navigasi layanan -->
<nav class="hidden sm:flex space-x-6 text-lg font-medium">
  <a href="#beranda" class="nav-link">Beranda</a>
  <a href="javascript:void(0)" onclick="openTentangKami()" class="nav-link">Tentang Kami</a>
  <a href="javascript:void(0)" onclick="openLayanan()" class="nav-link">Layanan</a>
  <a href="#kontak" class="nav-link">Kontak</a>
</nav>

<!-- Sembunyikan section layanan asli (opsional) -->
<section id="layanan" class="hidden"></section>

<!-- Kontak (dengan ikon sosial media) -->
<section id="kontak" class="py-20 bg-gray-100 px-6">
  <div class="max-w-4xl mx-auto text-center fade-in">
    <h2 class="text-3xl font-bold text-highlight mb-6">Kontak Kami</h2>
    <div class="flex justify-center space-x-6 text-2xl">
      <a href="mailto:lbhuit501@gmail.com" class="text-red-600 hover:text-red-800" title="Email">
        <i class="fas fa-envelope"></i>
      </a>
      <a href="https://wa.me/6285299383003" class="text-green-600 hover:text-green-800" title="WhatsApp">
        <i class="fab fa-whatsapp"></i>
      </a>
      <a href="https://www.facebook.com/LembagaBantuanHukumUit" class="text-blue-700 hover:text-blue-900" title="Facebook">
        <i class="fab fa-facebook"></i>
      </a>
      <a href="https://www.instagram.com/lembaga_bantuan_hukum_uit" class="text-pink-600 hover:text-pink-800" title="Instagram">
        <i class="fab fa-instagram"></i>
      </a>
    </div>
  </div>
</section>
