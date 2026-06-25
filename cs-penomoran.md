---
title: "Penomoran Otomatis"
description: "Panduan membuat kode unik atau ID referensi pelacakan (tracking ID) bagi setiap tiket aduan baru yang dibuat oleh pelanggan."
---

# 🔢 Penomoran Otomatis Tiket CS

Fitur **Penomoran Otomatis** pada CS Bot berfungsi untuk membuat kode unik atau ID referensi pelacakan (*tracking ID*) bagi setiap tiket aduan baru yang dibuat oleh pelanggan. 

Hasil dari format penomoran yang Anda rancang di sini akan secara otomatis diisi oleh AI ke dalam kolom **`Ticket Reference`** pada file Google Sheets Output atau basis data riwayat penanganan keluhan Anda.

![Kolom Ticket Reference pada Output Sheet CS](/assets/cs-penomoran-1.png)

---

## ⚠️ Syarat Mengaktifkan Kategori Tiket

Fitur Kategori Tiket ini **hanya akan berfungsi aktif** apabila Anda telah menyalakan sistem tiket utama pada panel kontrol CS Bot Anda.

![Pengaktifan Sistem Tiket CS](/assets/cs-kategori-2.png)

**Cara memastikannya:**

1. Pergi ke menu **Bot AI** > **CS Bot** > klik tab **Pengaturan** di panel kiri.
2. Pastikan sakelar pada menu **Aktifkan Sistem Tiket** berada dalam posisi **Aktif** (berwarna hijau). 
3. **Catatan:** Jika menu ini dinonaktifkan, seluruh percakapan yang masuk tidak akan dikelompokkan ke dalam tiket dan akan dialihkan langsung ke agen manusia.

---

## ⚙️ Cara Mengatur Format Penomoran Tiket

Setelah sistem tiket dipastikan aktif, Anda dapat merancang sendiri format kode referensi tiket yang ideal bagi tim *support* Anda.

![Halaman Konfigurasi Penomoran CS Bot](/assets/cs-penomoran-2.png)

### 1. Format Penomoran Utama
Di bagian kolom **Format Penomoran**, Anda dapat mengombinasikan berbagai variabel dinamis. Anda tidak perlu mengetik kodenya secara manual, cukup gunakan tombol bantu yang disediakan:

* Klik tombol **+ Tambahkan Kode** di sisi kanan kolom input.
* Pilih variabel penanda waktu yang diinginkan, seperti format **[NUMBER]** (Nomor Urut), **[MONTH]** (Angka/Romawi/Nama Bulan), hingga **[YEAR]** (Tahun).
* Gunakan indikator pratinjau (*Preview*) berwarna hijau di bawah kolom untuk melihat contoh langsung dari wujud kode tiket Anda.

### 2. Pengaturan Angka dan Prefix
Guna menyelaraskan dengan sistem pengarsipan internal perusahaan, Anda dapat mengonfigurasi detail deret angka:

* **Nomor Berikutnya:** Masukkan angka awal untuk memulai antrean tiket selanjutnya. Jika sistem baru dioperasikan, Anda bisa mengisinya dengan angka `1`.
* **Jumlah Digit Angka:** Tentukan lebar digit nomor urut Anda. Batas minimal pengisian adalah **3 digit** (Contoh: input `3` untuk menghasilkan format `001`).
* **Prefix (Opsional):** Jika Anda ingin menyisipkan kode teks statis sebagai identitas pembeda di depan nomor tiket, silakan isi kolom ini (Contoh: `TKT/` atau `CS/`).

### 3. Jadwal Reset Nomor
Guna mempermudah tim penanganan masalah dalam melacak volume aduan per periode, Anda dapat mengatur siklus pengaturan ulang (*reset*) nomor urut ke angka awal:

* **Tidak pernah reset (Terus berlanjut):** Angka antrean tiket akan terus bertambah tanpa batas waktu.
* **Setiap bulan (Nomor kembali ke 1 di awal bulan):** Urutan nomor otomatis kembali ke angka `1` begitu memasuki bulan baru.
* **Setiap tahun (Nomor kembali ke 1 di awal tahun):** Urutan nomor otomatis kembali ke angka `1` begitu berganti tahun baru.

---

## 💾 Menyimpan Format Penomoran

Jika seluruh struktur kode referensi tiket dirasa sudah rapi dan sesuai standar operasional tim *helpdesk* Anda, klik tombol hijau **Simpan** pada kotak *Simpan Perubahan* di sebelah kanan layar.