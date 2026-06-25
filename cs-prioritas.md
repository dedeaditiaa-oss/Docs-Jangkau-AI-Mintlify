---
title: "Prioritas Tiket"
description: "Panduan menentukan tingkat urgensi setiap keluhan pelanggan yang masuk untuk penyaringan masalah otomatis."
---

# ⚡ Prioritas Tiket CS

Menu **Prioritas Tiket** pada CS Bot berfungsi untuk menentukan tingkat urgensi setiap keluhan pelanggan yang masuk. Label tingkat prioritas yang ditentukan di sini nantinya akan otomatis masuk ke dalam **kolom priority pada output Google Sheets** Anda untuk memudahkan tim *support* melakukan penyaringan (*filtering*) masalah.

![Halaman Konfigurasi Prioritas Tiket CS Bot](/assets/cs-prioritas-1.png)

---

## 🛠️ Langkah Pengaturan Tambah Prioritas

Untuk membuat aturan prioritas baru bagi kecerdasan buatan (AI), klik tombol **+ Tambah Prioritas** terlebih dahulu, lalu lengkapi komponen formulir berikut:

### 1. Nama prioritas 
*   **Fungsi:** Masukkan nama label tingkatan urgensi tiket yang ingin Anda buat.
*   **Contoh Pengisian:** Anda dapat membaginya menjadi tiga standar umum, yaitu `Rendah`, `Sedang`, atau `Tinggi`. Nama label yang Anda ketik di kolom ini akan dikirimkan secara presisi sebagai teks data di kolom *priority* pada Google Sheets.

### 2. Kondisi Prioritas
*   **Fungsi:** Masukkan instruksi kontekstual, aturan logika, atau kata kunci opisional yang menjadi parameter AI dalam menetapkan tingkat prioritas secara otomatis.
*   **Contoh Pola Instruksi Kondisi:**
    *   *Kondisi untuk Tinggi:* "Setel ke Tinggi jika pelanggan menggunakan kata kunci penipuan, uang hilang, gagal bayar, akun dibobol, atau salah transfer."
    *   *Kondisi untuk Sedang:* "Setel ke Sedang jika pelanggan mengeluhkan masalah keterlambatan kurir pengiriman, salah varian produk, atau resi tidak terlacak."
    *   *Kondisi untuk Rendah:* "Setel ke Rendah jika chat hanya berupa pertanyaan umum tentang jam operasional toko, cara pakai fitur, atau kritik saran."

---

## 💾 Menyimpan Perubahan

Setelah Anda selesai mengisi komponen Nama Prioritas dan Kondisi Prioritas di atas, jangan lupa untuk selalu mengklik tombol hijau **Simpan** pada kotak *Simpan Perubahan* di sebelah kanan layar.