---
layout: page
title: Jus Ceria – Pilihan Jus Buah Segar
---

<!-- Logo Halal di atas -->
<!-- Logo Halal Tanpa Border Kosong -->

<!-- Navigasi -->
<nav style="margin-bottom:28px;">
  <a href="#menu" style="padding:7px 15px; margin:0 6px; background:#ff6f00; color:#fff; border-radius:5px;">Menu</a>
  <a href="#promo" style="padding:7px 15px; margin:0 6px; background:#43a047; color:#fff; border-radius:5px;">Promo</a>
  <a href="#about" style="padding:7px 15px; margin:0 6px; background:#0275d8; color:#fff; border-radius:5px;">About</a>
  <a href="#alamat" style="padding:7px 15px; margin:0 6px; background:#d9534f; color:#fff; border-radius:5px;">Alamat</a>
</nav>

<!-- Section Promo -->
<div id="promo" style="background:#ffe066; padding:17px 18px; border-radius:7px; margin-bottom:32px;">
  <h2 style="color:#cc8800; margin-bottom:6px;">Promo Terbaru!</h2>
  <p style="color:#783b02;">Dapatkan diskon 20% untuk pembelian minimal 2 botol jus hingga akhir bulan ini.</p>
</div>

<!-- Section Menu Terbaru -->
<div id="menu-terbaru" style="margin-bottom:35px;">
  <h2 style="color:#ff9000; text-align:center;">Menu Terbaru</h2>
  <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px;">
    {% assign menu_terbaru = site.data.jus | slice: 0,3 %}
    {% for jus in menu_terbaru %}
      <div style="width:210px; background:#fffbe6; border-radius:12px; border:2px solid #ffe066; box-shadow:0 2px 8px #eee; padding:13px 10px; text-align:center;">
        <img src="{{ jus.gambar }}" alt="{{ jus.judul }}" style="width:80px; height:80px; object-fit:cover; border-radius:50%; margin-bottom:10px;">
        <h4 style="color:#ff6f00;">{{ jus.judul }}</h4>
        <div style="color:#444; font-size:0.97em;">{{ jus.deskripsi }}</div>
      </div>
    {% endfor %}
  </div>
</div>

<!-- Section Semua Menu -->
<div id="menu" style="margin-bottom:35px;">
  <h2 style="color:#43a047; text-align:center;">Semua Menu Jus Kami</h2>
  <div style="display:flex; flex-wrap:wrap; justify-content:center; gap:20px;">
    {% for jus in site.data.jus %}
      <div style="width:200px; background:#f5f5f5; border-radius:10px; border:1px solid #ffe066; box-shadow:0 2px 8px #eee; padding:13px 10px; text-align:center; margin-bottom:10px;">
        <img src="{{ jus.gambar }}" alt="{{ jus.judul }}" style="width:65px; height:65px; border-radius:50%; margin-bottom:8px;">
        <h4 style="color:#ff6f00;">{{ jus.judul }}</h4>
        <div style="font-size:0.92em; color:#666;">{{ jus.deskripsi }}</div>
      </div>
    {% endfor %}
  </div>
</div>

<!-- Section About -->
<!-- Section About dengan Logo Halal Sejajar -->
<div id="about" style="margin-bottom:40px; background:#e3f2fd; border-radius:11px; padding:18px 15px; display:flex; align-items:center; gap:22px;">
  <div style="flex:1;">
    <h2 style="color:#0275d8;">Tentang Jus Ceria</h2>
    <p>Jus Ceria menghadirkan berbagai pilihan jus buah segar dengan resep alami, tanpa bahan pengawet dan pewarna buatan, cocok untuk semua generasi.</p>
  </div>
  <div style="flex-shrink:0;">
    <img src="/images/logo-halal.png"
     alt="Logo Halal"
     style="height:64px; display:block; background:none; box-shadow:none; border:none; margin:auto; padding:0;"/>

  </div>
</div>


<!-- Section Alamat -->
<!-- Section Alamat dan Kontak -->
<div id="alamat" style="margin-bottom:33px; background:#fff3e3; border-radius:12px; padding:19px 17px; box-shadow:0 2px 8px #eee;">
  <h2 style="color:#d9534f; font-size:1.22em; margin-bottom:10px;">Alamat & Kontak</h2>
  <p style="font-size:0.79em; color:#5a4633; font-family:'Lora', serif; margin-bottom:16px; line-height:1.6;">
    Temukan kami di lokasi strategis dan nyaman:<br>
    <span style="font-weight:600; color:#d9534f">
    <a href="https://maps.google.com/?q=Jl.+Pintu+Seng,+RT.12%2FRW.15,+Kapuk,+Kecamatan+Cengkareng,+Kota+Jakarta+Barat,+Daerah+Khusus+Ibukota+Jakarta+11720"
       target="_blank" style="color:#d9534f; text-decoration:none;">
      Jl. Pintu Seng, RT.12/RW.15,<br>
      Kapuk, Kecamatan Cengkareng,<br>
      Kota Jakarta Barat,<br>
      Daerah Khusus Ibukota Jakarta 11720
    </a>
    </span>
    <br>
    <span style="font-weight:600; color:#43a047;">
      WhatsApp/Phone:
      <a href="https://wa.me/628999563485" target="_blank" style="color:#43a047; text-decoration:none;">
        0899-9563-485
      </a>
    </span>
    <br>
    <span style="font-weight:500;">
      Provinsi :
      <a href="https://www.google.com/search?q=DKI+Jakarta+Province" target="_blank" style="color:#0275d8; text-decoration:none;">
        Jakarta
      </a>
    </span>
  </p>

  <!-- Social Media PNG Icons tanpa garis bawah -->
  <div style="margin-top:2px;">
    <a href="https://wa.me/628999563485" target="_blank" title="WhatsApp" style="margin-right:15px; text-decoration:none;">
      <img src="/images/wa.png" alt="WhatsApp" style="height:27px; vertical-align:middle;"/>
    </a>
    <a href="https://facebook.com/jusceria.id" target="_blank" title="Facebook" style="margin-right:15px; text-decoration:none;">
      <img src="/images/fb.png" alt="Facebook" style="height:27px; vertical-align:middle;"/>
    </a>
    <a href="https://instagram.com/jusceria.id" target="_blank" title="Instagram" style="margin-right:15px; text-decoration:none;">
      <img src="/images/ig.png" alt="Instagram" style="height:27px; vertical-align:middle;"/>
    </a>
    <a href="https://www.tiktok.com/@jusceria.id" target="_blank" title="TikTok" style="text-decoration:none;">
      <img src="/images/tiktok.png" alt="TikTok" style="height:27px; vertical-align:middle;"/>
    </a>
  </div>
</div>

</div>


</div>

