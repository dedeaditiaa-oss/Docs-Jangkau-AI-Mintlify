---
title: "Pengaturan Bot Sales"
description: "Panduan mengonfigurasi tingkat kreativitas respons AI, batas waktu tindak lanjut otomatis (idle), serta fitur pengingat pasca-pembayaran."
---

Menu **Pengaturan** pada Bot Sales digunakan untuk mengontrol perilaku bot saat berinteraksi dengan pelanggan, manajemen waktu operasional tindak lanjut otomatis, serta aktivasi fitur pengingat transaksi.

![Pengaturan Konfigurasi Bot Sales](/assets/sales-pengaturan-1.png)

---

## ⚙️ Komponen Konfigurasi Utama

### 1. Tunda Balasan Bot

* Ketika fitur ini aktif dan Anda menyetel interval contoh : **30 detik**, Bot akan menunggu selama 30 detik sejak pesan pertama masuk.
* Jika dalam masa tunggu tersebut pelanggan mengirimkan pesan tambahan, penghitung (*timer*) akan otomatis diulang kembali dari awal.
* Setelah pelanggan berhenti mengirimkan pesan, Bot akan menggabungkan seluruh pesan tersebut, membacanya secara utuh, dan mengirimkan jawaban yang relevan.

### 2. Tingkat Kreativitas
Fitur ini menentukan seberapa luwes atau ekspresif gaya bahasa yang digunakan oleh bot dalam merespons pesan percakapan dari calon pembeli.
* **Rendah Sekali / Rendah:** Bot akan membalas pesan secara kaku, baku, dan sangat disiplin hanya menggunakan data referensi produk yang Anda berikan.
* **Tinggi / Tinggi Sekali:** Bot akan membalas dengan gaya bahasa yang lebih ekspresif, imajinatif, dan kreatif dalam merangkai kalimat penawaran penjualan.

### 3. Follow Up Setelah Idle
Fitur otomasi bot apabila calon pelanggan tiba-tiba berhenti membalas chat. Jika dinyalakan, nantinya bot akan melakukan follow up sesuai dengan rentang waktu yang ditentukan. Jika dimatikan, nantinya bot tidak akan melakukan follow up jika pelanggan tidak membalas chat
* **Batas Waktu Idle:** Anda dapat menentukan rentang waktu tunggu (misalnya: `30 menit`). Jika pelanggan tidak mengirimkan aktivitas chat baru hingga batas waktu tersebut habis, bot secara otomatis akan mengirimkan pesan tindak lanjut (*follow-up*) untuk memicu kembali obrolan penjualan.

### 4. Reminder Otomatis

* **Fungsi:** Bot akan mengirimkan pesan pengingat (*reminder*) kepada pelanggan sesaat setelah pembayaran mereka dikonfirmasi dan diverifikasi oleh sistem internal Anda.
* Geser tombol ke **Aktif** untuk menyalakan fitur, atau geser ke **Nonaktif** jika Anda tidak ingin mengirimkan pesan pengingat otomatis pasca-pembayaran.

---

⚠️ **Langkah Terakhir:** Setiap kali Anda selesai mengubah kombinasi skala kreativitas, batas waktu, atau status pengingat, pastikan untuk menekan tombol hijau **Simpan** yang terletak di panel kartu **Simpan Perubahan** sebelah kanan agar pengaturan bot Anda langsung terbarui.