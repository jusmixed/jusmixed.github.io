---
layout: page
title: Jus Ceria – Pilihan Jus Buah Segar
---

<div style="text-align:center; margin-bottom:28px;">
  <h1 style="font-size:2em; color:#ff9000; font-weight:900; margin-bottom:4px;">Jus Ceria</h1>
  <div style="font-size:1.1em; color:#43a047;">Pilihan Jus Segar, Fresh & Alami</div>
  <nav style="margin:16px 0;">
    <a href="/" style="padding:7px 15px; margin:0 6px; background:#ff6f00; color:#fff; border-radius:5px;">Home</a>
    <a href="javascript:history.back()" style="padding:7px 15px; margin:0 6px; background:#43a047; color:#fff; border-radius:5px;">Back</a>
    <a href="#kategori" style="padding:7px 15px; margin:0 6px; background:#ffbf00; color:#fff; border-radius:5px;">Kategori</a>
    <a href="#about" style="padding:7px 15px; margin:0 6px; background:#0275d8; color:#fff; border-radius:5px;">About</a>
    <a href="#alamat" style="padding:7px 15px; margin:0 6px; background:#d9534f; color:#fff; border-radius:5px;">Alamat</a>
  </nav>
</div>

<!-- Grid 9 Jus -->
<div style="display:flex; flex-wrap:wrap; justify-content:center; gap:24px; margin-bottom:40px;">
  {% assign jusitems = site.data.jus %}
  {% for jus in jusitems %}
  <div style="width:250px; background:#fffbe6; border-radius:14px; border:2px solid #ffe066; box-shadow:0 2px 8px #eee; padding:14px 12px 16px 12px; text-align:center; margin-bottom:18px;">
    <a href="{{ jus.url }}">
      <img src="{{ jus.gambar }}" alt="{{ jus.judul }}" style="width:90px; height:90px; object-fit:cover; border-radius:50%; border:3px solid #ffbf00; margin-bottom:10px;">
    </a>
    <h3 style="font-size:1.1em; color:#ff6f00; margin-bottom:7px; margin-top:2px; font-weight:700;">
      <a href="{{ jus.url }}" style="color:#ff6f00;">{{ jus.judul }}</a>
    </h3>
    <div style="color:#666; font-size:0.97em; margin-bottom:2px;">{{ jus.deskripsi }}</div>
    <a href="{{ jus.url }}" style="background:#43a047; color:#fff; padding:5px 15px; border-radius:6px; margin-top:6px; display:inline-block;" target="_blank">Lihat Detail</a>
  </div>
  {% endfor %}
</div>
