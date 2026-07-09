---
title: "Katalog Produk"
description: "Panduan integrasi Google Sheets untuk mengelola katalog produk, melacak pesanan, serta mengatur notifikasi instan tim internal."
---

Menu **Katalog Produk** merupakan langkah paling awal dalam mengonfigurasi Bot Sales Anda. Di sini, Anda akan menghubungkan basis data toko anda menggunakan Google Sheets agar sinkronisasi produk, pelacakan keranjang, dan rekaman pesanan pelanggan dapat berjalan otomatis.

---

## 🔑 Langkah 1: Autentikasi Akun Google

Sebelum mengelola data, Anda wajib memberikan izin akses tautan ke akun Google Anda agar sistem dapat membuat lembar kerja otomatis.

1. Masuk ke halaman **Konfigurasi Bot Sales** dan pilih menu **Katalog Produk**.
2. Klik tombol hijau **Mulai Autentikasi dengan Google**.
3. Selesaikan proses login dan berikan izin akses pada *pop-up* akun Google yang muncul.

![Halaman Tautan Awal Google Sheets](/assets/sales-katalog-1.png)

---

## 📑 Langkah 2: Mengelola Lembar Kerja (Sheets)

Setelah proses autentikasi berhasil, tampilan dasbor Anda akan berubah menampilkan akses penuh ke lembar kontrol inventaris dan transaksi.

![Panel Manajemen Google Sheets yang Terhubung](/assets/sales-katalog-2.png)

### 📥 1. Input Sheet Katalog Produk
Klik tombol **Buka Sheet** pada bagian **Input Sheet Katalog Produk** untuk mengisi data barang dagangan Anda. Di dalam tabel ini, terdapat aturan pengisian kolom sebagai berikut:

* **Kolom Wajib Isi (Tanda Bintang \*):** **SKU\***, **Nama Produk\***, **Harga\***, dan **Stok\*** harus terisi agar sistem AI tidak salah membaca ketersediaan barang.
* **Kolom Opsional:** Kolom **Deskripsi** dan **Link Gambar Produk** bisa Anda isi untuk membantu Bot AI menjelaskan detail produk secara visual kepada calon pembeli di chat.

![Struktur Pengisian Input Sheet Katalog](/assets/sales-katalog-3.png)

> ⚠️ **PENTING:** Setiap kali Anda selesai mengubah, menambah, atau memperbarui data (seperti stok atau harga) langsung di Google Sheets, pastikan untuk kembali ke dasbor Jangkau AI dan klik tombol **🔄 Sinkron dari Sheet** agar data terbaru langsung diterapkan ke ingatan Bot.

---

### 📤 2. Output Sheet Pelacakan Pesanan
Apabila Anda mengklik tombol **Buka Sheet** di bagian **Output Sheet Pelacakan Pesanan**, Anda akan diarahkan ke buku kerja yang menampung 3 jenis sheet otomatis:

1. **Sheet Keranjang :** Menyimpan daftar barang belanjaan milik pelanggan yang sedang aktif. Sheet ini berjalan secara otomatis apabila Anda menyalakan fitur *Konfigurasi Keranjang*.
2. **Sheet Pesanan :** Rekaman detail setiap transaksi yang masuk, lengkap beserta Order ID, status pengiriman, total harga, hingga metode pembayaran pembeli.
3. **Sheet Keluhan :** Menampung rangkuman tiket keluhan operasional pelanggan jika ada kendala di lapangan.

| Nama Sheet | Ilustrasi Tampilan Output Data |
| :--- | :--- |
| **Keranjang** | ![Sheet Keranjang Otomatis](/assets/sales-katalog-4.png) |
| **Pesanan** | ![Sheet Data Pesanan Masuk](/assets/sales-katalog-5.png) |
| **Keluhan** | ![Sheet Tiket Keluhan Pelanggan](/assets/sales-katalog-6.png) |

---

## 🔔 Langkah 3: Pengaturan Notifikasi Tim Internal

Agar tim Anda bisa langsung memproses begitu ada transaksi atau aktivitas baru, Anda bisa menyalakan sistem pengingat otomatis.

1. Pada bagian bawah panel, klik tombol **➕ Tambah Notifikasi**.
2. Konfigurasikan formulir pengiriman seperti gambar acuan di bawah ini:
   * **Platform Pengirim:** Pilih platform obrolan yang akan ditugaskan mengirim pesan info notifikasi.
   * **Kategori (Opsional):** Centang aktivitas apa saja yang ingin Anda ketahui perkembangannya (contoh: *Pesanan Dibuat*, *Pembayaran Dibuat*, *Keranjang Dibuat*, dll.).
   * **Tipe Pesan:** Pilih **Pesan Pribadi** jika ingin dikirim langsung ke nomor admin tertentu (lalu masukkan nomor tujuan), atau pilih **Pesan Grup** apabila Anda ingin notifikasi tersebut masuk ke grup chat internal koordinasi tim.

![Formulir Penyiapan Notifikasi Internal](/assets/sales-katalog-7.png)

### 📝 Format & Contoh Hasil Pesan
Sistem menggunakan tag variabel `{{content_summary}}` yang wajib ada untuk menarik seluruh rangkuman pesanan dari obrolan pelanggan. 

Ketika notifikasi otomatis masuk ke platform tim internal Anda, struktur teks pesan rinciannya akan tampil rapi seperti berikut:

![Contoh Teks Notifikasi Transaksi Masuk](/assets/sales-katalog-8.png)

Jangan lupa klik **Simpan** setelah seluruh alur notifikasi internal selesai Anda konfigurasi dengan benar!