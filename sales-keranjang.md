---
title: "Konfigurasi Keranjang"
description: "Panduan mengaktifkan fitur keranjang belanja agar pelanggan dapat memesan beberapa produk sekaligus dalam satu kali checkout."
---

Menu **Konfigurasi Keranjang** pada Bot Sales berfungsi untuk mengatur apakah pelanggan diperbolehkan memilih beberapa item produk terlebih dahulu sebelum melakukan proses pembayaran.

![Halaman Konfigurasi Keranjang Belanja](/assets/sales-keranjang-1.png)

---

## 🛒 Mengatur Status Keranjang Belanja

Fitur ini dapat Anda sesuaikan dengan toko Anda:

### 1. Kondisi Aktif (Direkomendasikan untuk Multi-Produk)
Jika Anda menyalakan **Aktifkan Keranjang Belanja** :
* **Alur di Bot:** Pelanggan dapat memilih satu produk, menyimpannya sementara, memilih produk lain yang berbeda, lalu melakukan pembayaran untuk semua item tersebut secara bersamaan dalam satu proses.
* **Kelebihan:** Cocok untuk toko yang menjual banyak variasi produk (seperti retail, fashion, kosmetik, atau makanan) karena dapat meningkatkan nilai rata-rata keranjang belanja.

### 2. Kondisi Nonaktif (Direct Checkout)
Jika Anda mematikan saklar tersebut:
* **Alur di Bot:** Sistem keranjang akan dinonaktifkan. Setiap kali pelanggan memilih sebuah produk, Bot AI akan langsung mengarahkan mereka ke proses pengisian alamat dan pembayaran untuk produk itu saja.
* **Kelebihan:** Sangat cocok jika toko Anda hanya menjual produk tunggal, layanan jasa, atau produk digital yang umumnya dibeli satu per satu tanpa perlu digabung dengan item lain.

---

## 💾 Menyimpan Pengaturan

1. Sesuaikan posisi saklar **Aktifkan Keranjang Belanja** dengan kebutuhan transaksi toko Anda.
2. Jika sudah selesai, klik tombol hijau **✓ Simpan** pada panel kartu kanan atas untuk menerapkan konfigurasi tersebut ke sistem Bot AI secara langsung.