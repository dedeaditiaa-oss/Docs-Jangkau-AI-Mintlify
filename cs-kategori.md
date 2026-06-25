---
title: "Kategori Tiket"
description: "Panduan mengelompokkan setiap keluhan, kendala, atau pertanyaan bantuan pelanggan ke dalam label klasifikasi."
---

# 🏷️ Kategori Tiket CS

Fitur **Kategori Tiket** pada CS Bot berfungsi untuk mengelompokkan setiap keluhan, kendala, atau pertanyaan bantuan pelanggan ke dalam label klasifikasi. Dengan membagi tiket ke dalam kategori yang tepat, tim *Customer Service* dapat memetakan eskalasi masalah secara rapi dan mempercepat waktu penyelesaian kendala (*SLA*).

![Halaman Kategori Tiket CS Bot](/assets/cs-kategori-1.png)

---

## ⚠️ Syarat Mengaktifkan Kategori Tiket

Fitur Kategori Tiket ini **hanya akan berfungsi aktif** apabila Anda telah menyalakan sistem tiket utama pada panel kontrol CS Bot Anda.

![Pengaktifan Sistem Tiket CS](/assets/cs-kategori-2.png)

**Cara memastikannya:**

1. Pergi ke menu **Bot AI** > **CS Bot** > klik tab **Pengaturan** di panel kiri.
2. Pastikan sakelar pada menu **Aktifkan Sistem Tiket** berada dalam posisi **Aktif** (berwarna hijau). 
3. **Catatan:** Jika menu ini dinonaktifkan, seluruh percakapan yang masuk tidak akan dikelompokkan ke dalam tiket dan akan dialihkan langsung agen manusia.

---

## 🗂️ Cara Mengatur Kategori Masalah

Setelah sistem tiket dipastikan aktif, Anda dapat mulai merancang pengelompokan masalah pada menu **Kategori Tiket**. Terdapat dua kolom isian utama yang wajib Anda lengkapi pada setiap blok kategori:

* **Nama Kategori (Wajib):** Isi dengan nama klasifikasi masalah utama yang terjadi di lapangan. (Contoh: *Masalah Teknis*, *Komplain Pengiriman*, *Permintaan Refund*, *Pertanyaan Umum*).
* **Kondisi Kategori:** Masukkan instruksi logis, konteks, atau kata kunci panduan agar Bot AI dapat mendeteksi kapan sebuah obrolan harus dimasukkan ke kategori ini.
    * *Contoh Kondisi:* "Pilih kategori ini jika pelanggan mengeluhkan barang rusak saat sampai, kemasan jebol, paket salah kirim, atau kurir belum mengantarkan barang hingga melewati estimasi."

---

## ➕ Menambah & Menghapus Kategori Tiket

* **Tambah Kategori:** Anda dapat membuat banyak klasifikasi tiket sesuai kompleksitas operasional pusat bantuan Anda. Cukup klik tombol **+ Tambah Kategori** di bagian bawah halaman untuk memunculkan formulir baru.
* **Hapus Kategori:** Jika ada alur operasional yang berubah atau kategori yang ingin disederhanakan, Anda dapat menghapusnya dengan mengklik ikon **tempat sampah** berwarna merah di pojok kanan atas masing-masing blok kategori.

---

## 💾 Menyimpan Struktur Kategori

Setelah menyelesaikan pemetaan seluruh kategori kendala beserta indikator kondisinya, klik tombol hijau **Simpan** pada panel sebelah kanan. Langkah ini memastikan CS Bot Anda langsung mengenali jenis-jenis masalah baru dan siap melakukan klasifikasi tiket secara otomatis saat melayani pelanggan.