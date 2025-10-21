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
<div id="alamat" style="margin-bottom:33px; background:#fff3e3; border-radius:12px; padding:16px 15px;">
  <h2 style="color:#d9534f; font-size:1.15em;">Alamat & Kontak</h2>
  <p style="font-size:1.05em; margin-bottom:10px;">
    <a href="https://maps.google.com/?q=Jl.+Pintu+Seng,+RT.12%2FRW.15,+Kapuk,+Kecamatan+Cengkareng,+Kota+Jakarta+Barat,+Daerah+Khusus+Ibukota+Jakarta+11720"
       target="_blank" style="color:#d9534f; font-weight:600; text-decoration:underline;">
      Jl. Pintu Seng, RT.12/RW.15, Kapuk, Kecamatan Cengkareng, Kota Jakarta Barat, Daerah Khusus Ibukota Jakarta 11720
    </a><br>
    Phone/WA:
    <a href="https://wa.me/628999563485" target="_blank" style="color:#43a047; font-weight:600; text-decoration:underline;">
      0899-9563-485
    </a><br>
    Province:
    <a href="https://www.google.com/search?sca_esv=fbaa7d3b9c35fdd6&sxsrf=AE3TifMbAP6JhyMbjCeNLwgsx971jPnZkg:1761040179620&q=DKI+Jakarta+Province&si=AMgyJEuDKtOmISa9Akvtd6wQceP6KMdyloFoUI5CI2g3z4vsMT9nSuQavgbxJWMyZmPYW9tyOXeK-jORxVxsdMhWx1r9hOcAg1nK9kogVB0w8nTq2v7lFjcM9QFkTQa2Dyjaf54XIgcb3IKmJG5B-KYG77NFNH77nQ0YxB73OtmR79nHKOgkNDYDt724-TZHHHmchG6b2kt10iG2hJDGo_CFtJKq9wJcGw%3D%3D&sa=X&sqi=2&ved=2ahUKEwiUsd3ygbWQAxW4yzgGHeeODbgQmxN6BAglEAI" target="_blank" style="color:#0275d8; text-decoration:underline;">
      Jakarta
    </a>
  </p>
  <!-- Social Media -->
  <div style="margin-top:8px;">
  <a href="https://wa.me/628999563485" target="_blank" title="WhatsApp" style="margin-right:12px; font-size:1.2em;">🟢</a>
  <a href="https://facebook.com/jusceria.id" target="_blank" title="Facebook" style="margin-right:12px; font-size:1.2em;">🔵</a>
  <a href="https://instagram.com/jusceria.id" target="_blank" title="Instagram" style="margin-right:12px; font-size:1.2em;">🟣</a>
  <a href="https://www.tiktok.com/@jusceria.id" target="_blank" title="TikTok" style="font-size:1.2em;">⚫️</a>
</div>

</div>

