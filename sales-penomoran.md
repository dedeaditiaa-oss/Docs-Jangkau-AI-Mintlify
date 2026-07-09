---
title: "Penomoran Otomatis"
description: "Panduan mengatur format kode unik transaksional (Order ID) secara dinamis untuk setiap pesanan baru."
---

Menu **Penomoran Otomatis** pada Bot Sales digunakan untuk menentukan standardisasi format kode referensi pemesanan (**Order ID**). Format nomor yang rapi dan terstruktur dapat membantu tim admin atau operasional Anda dalam melacak, memvalidasi, serta mengarsipkan riwayat transaksi pembeli.


![Halaman Konfigurasi Penomoran Otomatis](/assets/sales-penomoran-1.png)

---

## ⚙️ Mengatur Komponen Format Order ID

Anda dapat menyusun kerangka nomor invoice pesanan dengan mengombinasikan beberapa variabel dinamis melalui kolom-kolom berikut:

### 1. Format Penomoran & Kode Dinamis
Pada kolom **Format Penomoran**, Anda bisa menyusun struktur kode menggunakan teks manual dan tag dinamis. Klik tombol **+ Tambahkan Kode** di sisi kanan untuk menyisipkan variabel otomatis seperti:
* `[NUMBER]`: Menyisipkan urutan angka transaksi saat ini.
* `[MONTH]`: Menyisipkan bulan berjalan saat transaksi terjadi (dalam angka).
* `[YEAR]`: Menyisipkan tahun berjalan saat transaksi terjadi.

> 💡 **Contoh:** Struktur `[NUMBER]/[MONTH]/[YEAR]` akan menghasilkan format Order ID seperti **001/07/2026**.

### 2. Parameter Urutan Angka
* **Nomor Berikutnya (Wajib):** Isikan angka awal dimulainya sistem penomoran baru (Default: `1`). Kolom ini akan bertambah secara otomatis (+1) setiap kali ada pesanan masuk.
* **Jumlah Digit Angka:** Tentukan berapa total digit minimal untuk nomor urut (Minimal: `3`). Jika diisi `3`, angka urutan akan memuat awalan nol (contoh: angka 1 menjadi `001`, angka 25 menjadi `025`).
* **Prefix (Opsional):** Tambahkan teks penanda khusus di bagian depan kode jika diperlukan (Contoh: `ORD/` atau `INV-`).

---

## 🔄 Jadwal Reset Nomor

Tentukan kapan sistem harus mengembalikan urutan angka penomoran kembali ke awal (`1`):

* **Tidak pernah reset (Terus berlanjut):** Angka urutan transaksi akan terus membesar tanpa batas waktu (Contoh: ...099, 100, 101, dst.).
* **Setiap bulan:** Urutan nomor otomatis dikembalikan menjadi `1` setiap kali memasuki tanggal 1 di bulan baru.
* **Setiap tahun:** Urutan nomor otomatis dikembalikan menjadi `1` setiap kali memasuki tanggal 1 Januari di tahun baru.

---

## 💾 Menyimpan Format Penomoran

Periksa tampilan akhir format Order ID Anda pada bagian label **Preview**. Jika kombinasi kode dirasa sudah sesuai dengan skema penomoran internal perusahaan Anda, klik tombol hijau **✓ Simpan** pada panel kartu **Simpan Perubahan** di bagian kanan atas layar.