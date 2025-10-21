---
layout: page
title: Jus Ceria – Pilihan Jus Buah Segar
---

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
<div id="about" style="margin-bottom:40px;">
  <h2 style="color:#0275d8;">Tentang Jus Ceria</h2>
  <p>Jus Ceria menghadirkan berbagai pilihan jus buah segar dengan resep alami, tanpa bahan pengawet dan pewarna buatan, cocok untuk semua generasi.</p>
</div>

<!-- Section Alamat -->
<div id="alamat">
  <h2 style="color:#d9534f;">Alamat & Kontak</h2>
  <p>Jl. Sehat Segar No.88, Kota Buah, Indonesia<br>
     Telp/WA: 0812-3456-7890</p>
</div>
