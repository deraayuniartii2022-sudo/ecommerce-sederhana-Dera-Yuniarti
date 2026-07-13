# 🍫 Laporan Proyek Mandiri: E-Commerce Berbasis Web Statis "Choco Bites"

---

## 📌 PART 1: BUSINESS OVERVIEW (GAMBARAN UMUM BISNIS)
*Ringkasan cepat performa operasional komersial Choco Bites by Dera.*

* **Nama Bisnis:** Choco Bites by Dera
* **Value Proposition:** *"Premium Taste in Every Single Bite."* Menawarkan kue cokelat premium (fudgy brownies & matcha) bertekstur lumer dengan kemasan estetik dan harga ramah kantong.
* **Target Pasar Utama:** Remaja dan dewasa muda (15-30 tahun), pelajar/mahasiswa, pencinta makanan manis (*sweet tooth*), serta aktif di media sosial.
* **Model Pendapatan:** B2C (Direct-to-Consumer) melalui penjualan retail produk harian dan paket khusus/hampers hari raya secara online.
* **Link Website Resmi:** [Choco Bites by Dera Live](https://deraayuniartii2022-sudo.github.io/ecommerce-sederhana-Dera-Yuniarti/)

---

## 📋 PART 2: BUSINESS DOCUMENTATION (DOKUMENTASI BISNIS DETAIL)
*Analisis mendalam strategi, manajemen, dan proyeksi operasional usaha.*

### 1. Latar Belakang & Transformasi Digital
Choco Bites didirikan untuk menjawab tingginya permintaan pasar terhadap kudapan manis berkualitas tinggi. Guna meningkatkan skala pasar tanpa terbentur batas geografis dan meminimalkan biaya operasional (*overhead cost*), dilakukan transformasi ke ranah digital melalui platform e-commerce statis. Strategi ini menghadirkan etalase toko online yang super cepat, ringan, dan efisien.

### 2. Segmentasi Pelanggan & Analisis Pasar
* **Demografi & Geografi:** Berfokus pada masyarakat urban usia produktif (15-30 tahun) dengan tingkat konsumsi camilan manis yang tinggi.
* **Psikografi:** Konsumen yang gemar membagikan momen kuliner estetik ke media sosial (Instagram/TikTok) serta mencari bingkisan unik.
* **Kompetitor:** Toko bakery konvensional berskala besar. Choco Bites unggul dari segi variasi rasa modern (seperti autentisitas Matcha premium) dan kemudahan akses pemesanan digital.

### 3. Strategi Manajemen Produk & Katalog
Katalog produk dirancang terstruktur menggunakan visual beresolusi tinggi dengan pencahayaan hangat (*warm tone*) untuk meningkatkan *appetite appeal*:
* **Kategori Brownies Premium:** Fudgy brownies renyah di luar, lumer di dalam dengan pilihan topping sekat (almond, keju, choco chips).
* **Kategori Matcha Special:** Komposisi cokelat bar/brownies dengan sentuhan teh hijau Jepang asli untuk menyeimbangkan rasa manis.

### 4. Strategi Harga, Promosi, dan Diskon
* **Penetapan Harga:** Menggunakan *Value-Based Pricing* (menyesuaikan kualitas bahan baku premium namun tetap bersaing ketat dengan pasar lokal).
* **Taktik Promosi:** Memanfaatkan kekuatan *Social Media Marketing* (Instagram/TikTok Ads) untuk mengarahkan trafik potensial masuk ke website.
* **Program Diskon:** Implementasi strategi "Bundle Hemat" (pembelian multiproduk) serta promo gratis ongkir tematik pada hari-hari besar.

### 5. Arsitektur Transaksi (Checkout & Payment Gateway)
Untuk menghadirkan pengalaman belanja modern, platform dipersiapkan terintegrasi dengan simulator payment gateway **Midtrans (Sandbox Mode)** melalui alur:
1. **Pilih Produk:** Konsumen memilih varian menu dan menekan tombol "Beli Sekarang".
2. **Checkout Page:** Mengisi data pengiriman (Nama, Alamat lengkap, No. WhatsApp).
3. **Simulasi Pembayaran:** Sistem memicu *Pop-up* Midtrans Snap. Pengguna dapat memilih metode pembayaran dummy (Virtual Account Bank Mandiri/BCA, atau QRIS simulator).
4. **Verifikasi Otomatis:** Notifikasi dikirimkan ke sistem secara otomatis, merubah status pesanan menjadi "Lunas/Siap Dikirim".

### 6. Strategi SEO, Keamanan, dan Pemeliharaan Sistem
* **Optimasi SEO:** Memasang *Meta Keywords* dan *Meta Description* strategis (e-commerce brownies, brownies premium terdekat) pada file HTML agar mudah dirayap Google.
* **Protokol Keamanan:** Penyebaran web menggunakan enkripsi data ketat lewat jaringan **HTTPS (SSL Certificate)** bawaan GitHub Pages.
* **Pemeliharaan:** Pengujian berkala pada responsivitas tombol, validasi link transaksi, serta pembaharuan katalog visual berkala sebulan sekali.

### 7. Rencana Optimalisasi Data Analytics
Pengambilan keputusan bisnis ke depan sepenuhnya didasarkan pada data (*data-driven decision*):
* **Analisis Varian Terlaris:** Mengamati halaman produk paling diminati untuk menentukan efisiensi stok bahan baku.
* **Analisis Perilaku:** Evaluasi rasio pentalan pengunjung guna melakukan perbaikan berkelanjutan pada desain antarmuka.

---

## 🛠️ PART 3: TECHNICAL EXPLANATION (PENJELASAN TEKNIS SCRIPT)
*Arsitektur kode, integrasi pelacak data, dan infrastruktur kompilasi web.*

### 1. Arsitektur Kode & Penataan Responsif
Website dibangun dengan kombinasi **HTML5** sebagai kerangka semantik elemen web, serta **CSS3** sebagai pengatur tata letak visual. Kode stylesheet diperkuat dengan fitur *Media Queries* (`@media (max-width: 768px)`) untuk menjamin aspek *Responsive Web Design* (RWD) agar tampilan halaman otomatis beradaptasi secara dinamis saat diakses dari perangkat mobile (smartphone) maupun desktop.

### 2. Integrasi Google Analytics 4 (GA4)
Skrip pelacak dari Google Analytics disematkan secara global pada komponen utama `<head>` di dalam file `index.html` dengan ID Pelacak riil `G-SRV3K6SKSM`.

Berikut potongan kodenya:
```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Choco Bites by Dera</title>

<!-- Google tag (gtag.js) Integration -->
<script async src="[https://www.googletagmanager.com/gtag/js?id=G-SRV3K6SKSM](https://www.googletagmanager.com/gtag/js?id=G-SRV3K6SKSM)"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-SRV3K6SKSM');
</script>
