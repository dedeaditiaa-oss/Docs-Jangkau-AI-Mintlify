---
title: "Konfigurasi Pengiriman"
description: "Panduan lengkap mengelola alamat operasional toko, setup metode Kurir Toko (Radius/Area), serta opsi Ambil ke Toko (Self-Pickup)."
---

Menu **Konfigurasi Pengiriman** pada Bot Sales digunakan untuk menentukan lokasi fisik operasional bisnis Anda serta mengatur metode penyerahan barang kepada konsumen. Pengaturan alamat yang penting agar bot AI dapat menghitung opsi jangkauan pengiriman dan ongkos kirim secara otomatis saat melayani transaksi di ruang obrolan.

![Halaman Utama Konfigurasi Pengiriman](/assets/sales-pengiriman-1.png)

---

## 📍 Langkah 1: Menambahkan Alamat Toko

![Peta Penentuan Titik Koordinat Toko](/assets/sales-pengiriman-2.png)

![Peta Penentuan Titik Koordinat Toko](/assets/sales-pengiriman-3.png)

Sebelum mengaktifkan metode pengiriman, Anda wajib mendaftarkan alamat toko atau cabang Anda terlebih dahulu:


1. Klik tombol **➕ Tambah Alamat** atau **+ Tambah Alamat Sekarang**.
2. Isi kolom **Nama Toko/Cabang** (Contoh: *Toko Pusat*, *Gudang Jakarta*).
3. Masukkan **Alamat Lengkap** secara detail (Nama jalan, nomor bangunan, RT/RW, kecamatan, dan kota).
4. **Pilih Lokasi di Peta:** Ketikkan area umum Anda pada kolom pencarian Google Maps, lalu **geser pin merah** untuk menyesuaikan titik koordinat lokasi akurat toko Anda. Titik koordinat ini digunakan sebagai acuan perhitungan jarak radius pengiriman.


---

## 🚚 Langkah 2: Mengonfigurasi Metode Pengiriman

Setelah alamat berhasil disimpan, Anda dapat mengaktifkan dua jenis metode penyerahan produk di bawah ini sesuai kebutuhan operasional:

### A. Opsi Kurir Toko

![Pengaturan Detail Kurir Toko](/assets/sales-pengiriman-4.png)

Metode ini diaktifkan jika Anda memiliki armada pengiriman mandiri atau menggunakan kurir internal untuk mengantar pesanan langsung ke lokasi pembeli. Pilih tombol **Aktif (Hijau)** jika anda memiliki kurir sendiri :

* **Jam Operasional:** Atur waktu layanan pengiriman dengan menentukan batas jam **Buka** dan jam **Tutup** (Contoh: `08:00 AM` s.d `09:00 PM`).
* **Area Layanan:** Tentukan batasan jangkauan pengiriman kurir Anda:
  * **Radius (km):** Membatasi jangkauan titik peta toko (Misal: `5 km`).
  * **Ke Area Tertentu:** Membatasi jangkauan berdasarkan wilayah tertentu.
* **Biaya Pengiriman:** Pilih skema tarif yang ingin dibebankan kepada konsumen:
  * **Tarif Flat:** Ongkos kirim bernilai tetap sama ke mana pun dalam area layanan (Contoh: `Rp 5000`).
  * **Biaya per KM:** Ongkos kirim akan dikalikan secara otomatis berdasarkan jarak tempuh dari toko ke posisi pembeli.
* **Gratis Ongkir:** Aktifkan pengaturan ini jika Anda ingin memberikan promo bebas biaya kirim. Saat dinyalakan, Anda dapat mengatur parameter minimal nominal pembelanjaan tertentu agar pembeli mendapatkan gratis ongkir.
* **Estimasi Waktu Pengiriman:** Tuliskan estimasi waktu barang sampai ke pelanggan untuk diinformasikan oleh bot (Contoh: `1 jam setelah pembayaran`).


---

### B. Opsi Ambil ke Toko (Self-Pickup)

![Pengaturan Detail Ambil ke Toko](/assets/sales-pengiriman-5.png)

Metode ini diaktifkan jika Anda ingin memberikan kebebasan kepada pembeli untuk melakukan pemesanan secara daring melalui chat dan mengambil barangnya sendiri. Aktifkan pilihan untuk melakukan setup:

* **Jam Operasional:** Tentukan waktu operasional layanan pengambilan mandiri (Buka dan Tutup).
* **Estimasi Waktu Pickup:** Isi durasi waktu yang dibutuhkan oleh tim toko Anda untuk menyiapkan produk pesanan hingga siap diambil oleh pelanggan setelah divalidasi (Contoh: `1 jam setelah pembayaran`).

---

⚠️ **Langkah Terakhir:** Setelah selesai memasukkan data alamat serta menentukan rincian aturan kurir ataupun pickup, pastikan Anda menekan tombol hijau **Simpan Perubahan** yang berada pada panel kartu **Simpan Konfigurasi** di bagian kanan atas agar data operasional logistik bot diperbarui secara *real-time*.