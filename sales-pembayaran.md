---
title: "Metode Pembayaran"
description: "Panduan mengatur opsi pembayaran pelanggan via Bayar di Tempat (COD), Transfer Bank, dan kode QRIS otomatis."
---

Menu **Metode Pembayaran** pada Bot Sales berfungsi untuk menentukan bagaimana pelanggan dapat menyelesaikan transaksi pembelian. Anda bisa mengaktifkan salah satu metode, mengombinasikannya, atau langsung menyalakan ketiga metode pembayaran.

---

## 💵 Opsi 1: Bayar langsung di Tempat / COD

Metode ini memungkinkan pelanggan melakukan pemesanan terlebih dahulu dan menyelesaikan pembayaran secara tunai (cash) langsung saat barang mereka terima.

* **Cara Aktivasi:** Nyalakan pilihan **Bayar langsung di Tempat / COD** hingga berwarna hijau (Aktif).
* **Alur di Bot:** Saat bertransaksi, AI akan mengonfirmasi kepada pelanggan bahwa pesanan akan diproses dan pembayaran dilakukan secara langsung di toko atau saat kurir mengantarkan paket ke alamat tujuan.

![Aktivasi Metode Pembayaran COD](/assets/sales-pembayaran-1.png)

---

## 🏦 Opsi 2: Bank Transfer

Metode ini digunakan apabila Anda ingin menerima pembayaran melalui transfer antar-rekening bank. 

1. Nyalakan pilihan **Bank Transfer** ke posisi aktif (Hijau).
2. Klik tombol **➕ Tambah Rekening Bank** .
3. Masukkan informasi detail rekening Anda, seperti:
   * Nama Bank (Contoh: BCA, Mandiri, BRI, dll.)
   * Nomor Rekening
   * Nama Pemilik Rekening (Atas Nama)
4. **Alur di Bot:** Ketika pembeli memilih opsi ini, Bot AI secara otomatis mengirimkan rincian nomor rekening tujuan transfer Anda.

![Aktivasi Metode Pembayaran Bank Transfer](/assets/sales-pembayaran-2.png)

---

## 📱 Opsi 3: QRIS

Metode QRIS mempermudah pelanggan untuk membayar secara digital secara instan (Gopay, OVO, Dana, LinkAja) maupun mobile banking hanya dengan memindai kode QR.

1. Aktifkan menu **QRIS**
2. Pada kolom **QRIS Code** yang muncul, klik area bertuliskan **Unggah QRIS**.
3. Pilih dan masukkan gambar kode QRIS milik toko Anda (format gambar `.png` atau `.jpg`).
4. **Alur di Bot:** Saat proses pembelian, Bot AI akan langsung menampilkan gambar kode QRIS toko Anda sehingga pelanggan bisa langsung memindai QRIS tersebut.

![Aktivasi Metode Pembayaran QRIS](/assets/sales-pembayaran-3.png)

---

⚠️ **Langkah Penting:** Jangan lupa untuk menekan tombol **Simpan Perubahan** pada panel kartu **Simpan Konfigurasi** di bagian kanan atas layar setiap kali Anda selesai memperbarui, menambah, atau mengubah detail info rekening dan gambar QRIS Anda!