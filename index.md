---
layout: page
title: Jus Mixed – Pilihan Jus Buah Segar
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
    <h2 style="color:#0275d8;">Tentang Jus Mixed</h2>
    <p>Jus Mixed menghadirkan berbagai pilihan jus buah segar dengan resep alami, tanpa bahan pengawet dan pewarna buatan, cocok untuk semua generasi.</p>
  </div>
</div>


<!-- Section Alamat -->
<!-- Section Alamat dan Kontak -->
<!-- Section Alamat dan Kontak + Peta Google Maps -->
<div id="alamat" style="
  margin-bottom:33px;
  background:#fff3e3;
  border-radius:12px;
  padding:19px 17px;
  box-shadow:0 2px 8px #eee;
  display:flex;
  flex-wrap:wrap;
  gap:30px;
  align-items:flex-start;
">

  <!-- Alamat & Kontak -->
  <div style="flex:1; min-width:220px;">
    <h2 style="color:#d9534f; font-size:1.22em; margin-bottom:10px;">Alamat & Kontak</h2>
    <p style="font-size:1em; color:#5a4633; font-family:'Lora',serif; margin-bottom:18px; line-height:1.6; font-weight:600;">
      <b>Depan SDN Kapuk 09 Pagi:</b><br>
      <span style="color:#d9534f;">
        <a href="https://maps.google.com/?q=Jl.+Pintu+Seng,+RT.12%2FRW.15,+Kapuk,+Kecamatan+Cengkareng,+Kota+Jakarta+Barat,+Daerah+Khusus+Ibukota+Jakarta+11720" target="_blank" style="color:#d9534f; text-decoration:none;">
          Jl. Pintu Seng, RT.12/RW.15,<br>
          Kapuk, Kecamatan Cengkareng,<br>
          Kota Jakarta Barat,<br>
          Daerah Khusus Ibukota Jakarta 11720
        </a>
      </span>
      <br>
      <span style="color:#43a047;">
        WhatsApp/Phone:
        <a href="https://wa.me/628999563485" target="_blank" style="color:#43a047; text-decoration:none;">
          0899-9563-485
        </a>
      </span>
      <br>
      <span>
        Lokasi:
        <a href="https://www.google.com/search?q=DKI+Jakarta+Province" target="_blank" style="color:#0275d8; text-decoration:none;">
          Jakarta
        </a>
      </span>
    </p>

    <!-- Media Sosial & Food Platform -->
    <div style="margin-bottom:16px;">
      <a href="https://wa.me/628999563485" target="_blank" title="WhatsApp" style="margin-right:18px; text-decoration:none;">
        <img src="/images/wa.png" alt="WhatsApp" style="height:28px; vertical-align:middle;"/>
      </a>
      <a href="https://gofood.co.id/jakarta/restaurant/jusmixed-id-xxxx" target="_blank" title="GojekFood" style="margin-right:18px; text-decoration:none;">
        <img src="/images/gofood.png" alt="GoFood" style="height:28px; vertical-align:middle;"/>
      </a>
      <a href="https://shopee.co.id/universitas/jusmixed-id-xxxx" target="_blank" title="ShopeeFood" style="margin-right:18px; text-decoration:none;">
        <img src="/images/shopeefood.png" alt="ShopeeFood" style="height:28px; vertical-align:middle;"/>
      </a>
      <a href="https://tiktok.com/@jusmixedid" target="_blank" title="Tiktok" style="text-decoration:none;">
        <img src="/images/tiktok.png" alt="Tiktok" style="height:28px; vertical-align:middle;"/>
      </a>
      <a href="https://youtube.com/@jusmixedid" target="_blank" title="YouTube" style="text-decoration:none;">
        <img src="/images/youtube.png" alt="YouTube" style="height:28px; vertical-align:middle;"/>
      </a>
    </div>
  </div>

  <!-- Peta Google Maps -->
  <div style="min-width:240px; max-width:380px; flex:1; display:flex; justify-content:center;">
    <iframe
      src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3966.872476673503!2d106.73993007585969!3d-6.147824260265217!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f7e6232c99af%3A0xfbe8ab5a40450aa7!2sSDN%20Kapuk%2009%20Pagi%2C%2010%20Petang!5e0!3m2!1sen!2sid!4v1761200595203!5m2!1sen!2sid"
      width="100%"
      height="235"
      style="border:0; border-radius:16px; box-shadow:0 2px 12px #bbb;"
      allowfullscreen=""
      loading="lazy"
      referrerpolicy="no-referrer-when-downgrade">
    </iframe>
  </div>

</div>



