---
title: "Pengaturan"
description: "Panduan mengonfigurasi bagaimana cara bot AI mengelola keluhan pelanggan, mengatur alur pembuatan tiket bantuan, hingga menentukan tindakan tindak secara lanjut otomatis."
---

# ⚙️ Pengaturan CS Bot & Sistem Tiket

Menu **Pengaturan** pada CS Bot memungkinkan Anda untuk mengonfigurasi bagaimana cara bot AI mengelola keluhan pelanggan, mengatur alur pembuatan tiket bantuan, hingga menentukan tindakan tindak secara lanjut otomatis.

---

## 🎫 1. Aktivasi & Konfigurasi Sistem Tiket

Fitur ini merupakan pusat kendali utama untuk mengaktifkan atau menonaktifkan manajemen antrean keluhan terstruktur di dalam CS Bot Anda.

### 🔴 Kondisi Saat Sistem Tiket Dimatikan
Apabila **Aktifkan Sistem Tiket** berada dalam posisi **Tidak Aktif**, maka seluruh obrolan keluhan pelanggan akan dilemparkan langsung kepada agen manusia tanpa adanya pembuatan nomor antrean kasus. Tampilan fitur pendukung lainnya akan disembunyikan.

![Sistem Tiket Tidak Aktif](/assets/cs-pengaturan-1.png)

---

### 🟢 Kondisi Saat Sistem Tiket Dinyalakan
Apabila sakelar **Aktifkan Sistem Tiket** digeser ke posisi **Aktif** (berwarna hijau), sistem otomatis akan memunculkan beberapa opsi konfigurasi tambahan di bawahnya:

![Sistem Tiket Aktif](/assets/cs-pengaturan-2.png)

#### a. Kapan Tiket Dibuat
Pilihan ini menentukan momentum atau pemicu utama kapan nomor referensi tiket pelacakan kasus harus mulai diproduksi oleh bot. Menu *dropdown* ini menyediakan 2 pilihan mekanis:

* **Selalu buat tiket:** Begitu pelanggan mengirimkan pesan sapaan atau aduan pertama, bot langsung otomatis mengunci sesi tersebut ke dalam nomor referensi kasus baru.
* **Hanya jika bot tidak bisa menjawab:** Bot akan bekerja keras menjawab keluhan menggunakan basis pengetahuan QnA terlebih dahulu. Nomor tiket pelacakan baru akan diproduksi jika pelanggan menemui jalan buntu dan butuh bantuan agen manusia.

![Pilihan Pemicu Pembuatan Tiket](/assets/cs-pengaturan-3.png)

#### b. Reminder Otomatis
Fitur ini berfungsi agar bot bergerak secara proaktif guna menawarkan pesan pengingat (*reminder*) setelah memberikan panduan perawatan, jadwal janji temu, atau saran tindakan solusi tertentu kepada pelanggan.

* **Aktif:** Bot otomatis mengirimkan teks pengingat lanjutan agar pelanggan segera mengecek status penanganan masalah mereka.
* **Nonaktif:** Bot tidak mengirimkan tawaran pengingat 

![Mekanisme Reminder Otomatis](/assets/cs-pengaturan-4.png)

#### c. Integrasi Google Sheets
Opsi ini berfungsi untuk menghubungkan data tiket dari Bot CS Anda ke spreadsheet Google secara otomatis untuk mempermudah pengarsipan data. Proses integrasinya terbagi menjadi dua tahap tampilan:

* **Tampilan Sebelum Terhubung (Belum Aktif):** Pada tahap awal, sistem akan meminta otentikasi. Anda perlu mengklik tombol hijau **Connect Google Account** untuk memberikan izin akses pembuatan sheet output tiket.

![Integrasi Google Sheets - Belum Terhubung](/assets/cs-pengaturan-5.png)

* **Tampilan Setelah Terhubung (Sudah Aktif):** Setelah proses otentikasi akun Google berhasil, tampilan panel akan berubah menjadi **Google Account Connected**. Sistem akan segera membuat spreadsheet baru di akun Google Anda secara otomatis. Pada tampilan ini, Anda memiliki beberapa tombol aksi:
    * **Buka Sheet:** Untuk langsung membuka dokumen spreadsheet hasil output tiket.
    * **Coba dan Buat Ulang Sheets:** Untuk membuat ulang lembar kerja baru jika terjadi kendala.
    * **Putuskan Koneksi:** Tombol merah untuk memutuskan integrasi akun Google yang sedang aktif.

![Integrasi Google Sheets - Berhasil Terhubung](/assets/cs-pengaturan-6.png)

#### d. Pengaturan Notifikasi Tim Internal
Bagian ini digunakan apabila Anda ingin memantau masuknya tiket aduan atau keluhan baru dari pelanggan secara cepat. Setiap kali ada tiket baru dengan kriteria tertentu yang terpenuhi, sistem akan memicu alarm pemberitahuan otomatis ke tim internal Anda agar penanganan masalah (*troubleshooting*) dapat dilakukan secepat mungkin.

Untuk mengaktifkan fitur ini, setelah mengklik tombol **+ Tambah Notifikasi**, Anda perlu melengkapi komponen pengaturan berikut:

![Halaman Formulir Tambah Notifikasi Internal](/assets/cs-pengaturan-7.png)

* **Platform Pengirim:** Pilih platform atau saluran komunikasi yang akan digunakan sistem untuk mengirimkan pesan notifikasi ke tim Anda.
* **Kategori (Opsional):** Pilih jenis kategori masalah tiket apa saja (misalnya: Masalah Pembayaran, Bug Sistem) yang ingin Anda pantau untuk dikirimkan notifikasinya. Anda dapat memilih opsi **Semua** untuk memantau seluruh kategori.
* **Klasifikasi / Prioritas (Opsional):** Pilih tingkat urgensi tiket tertentu yang ingin Anda prioritaskan (misalnya hanya memicu notifikasi untuk tiket tingkat *High*). Anda dapat memilih opsi **Semua** jika ingin memantau setiap tingkatan prioritas.
* **Tipe Pesan:** Tentukan arah tujuan pengiriman alarm notifikasi. Terdapat 2 pilihan mekanisme:
    * **Pribadi:** Jika memilih tipe ini, Anda wajib memasukkan nomor pribadi tujuan. Informasi data tiket masuk nantinya hanya akan dikirimkan secara privat ke nomor tersebut.
    * **Grup:** Jika memilih tipe ini, informasi rangkuman tiket baru akan dikirimkan langsung ke dalam grup obrolan bersama, sehingga seluruh anggota tim *support* di dalam grup tersebut dapat mengetahuinya.
* **Isi Pesan:** Tulis template teks draf pesan notifikasi otomatis yang ingin Anda terima di saluran komunikasi tim internal.

Berikut adalah contoh format tampilan ringkasan notifikasi yang akan diterima oleh ponsel tim internal Anda ketika ada tiket aduan baru yang berhasil dicatat oleh AI:

![Halaman Formulir Tambah Notifikasi Internal](/assets/cs-pengaturan-8.png)

---
## 2. Tunda Balasan Bot

Tunda balasan bot berfungsi agar bot anda tidak langsung membalas pesan dari pelanggan

![Tunda balasan bot](/assets/cs-pengaturan-bot.png)

### 💡 Cara Kerja Sistem:
* Ketika fitur ini aktif dan Anda menyetel interval contoh : **30 detik**, Bot akan menunggu selama 30 detik sejak pesan pertama masuk.
* Jika dalam masa tunggu tersebut pelanggan mengirimkan pesan tambahan, penghitung (*timer*) akan otomatis diulang kembali dari awal.
* Setelah pelanggan berhenti mengirimkan pesan, Bot akan menggabungkan seluruh pesan tersebut, membacanya secara utuh, dan mengirimkan jawaban yang relevan.

## ✨ 3. Tingkat Kreativitas AI

Pengaturan skala kreativitas mengontrol seberapa kaku atau seberapa luwes gaya bahasa AI saat memberikan batasan kepada konsumen Anda. 

![Skala Kreativitas AI](/assets/cs-pengaturan-9.png)

Anda dapat menentukan tingkatan respons melalui pilihan *dropdown* berikut:

* **Rendah Sekali / Rendah:** Bot akan merespons dengan kalimat yang sangat formal, kaku,  dan konsisten berdasarkan teks dokumen baku.
* **Normal:** (Rekomendasi) Gaya bahasa penanganan keluhan yang seimbang; ramah, solutif, natural, namun tetap menjaga profesionalisme layanan.
* **Tinggi / Tinggi Sekali:** Bot akan menggunakan kosakata yang jauh lebih ekspresif, variatif, dan luwes saat memberikan jawaban ke konsumen.

---

## ⏱️ 4. Follow Up Setelah Idle

Fitur ini berfungsi untuk mengatasi masalah operasional di mana pelanggan tiba-tiba berhenti membalas percakapan (*idle*).

![Konfigurasi Batas Idle](/assets/cs-pengaturan-10.png)

* **Fungsi:** Apabila dinyalakan, Jika pelanggan tidak merespons dalam rentang waktu tertentu, bot akan otomatis mengirimkan pesan sapaan hangat/konfirmasi lanjutan untuk memancing balik respons mereka agar tiket kasus tidak hangus atau kedaluwarsa. Jika Idle dimatikan, nantinya Bot tidak akan melakukan follow up apabila pelanggan tidak membalas
* **Batas Waktu Idle:** Anda dapat memilih durasi waktu tunggu bot yang sesuai dengan SOP bisnis Anda melalui pilihan menu:
    * `5 menit`   
    * `10 menit`
    * `30 menit`
    * `1 jam`
    * `2 jam`
    * `24 jam`

---

## 💾 Menyimpan Perubahan

Setiap kali Anda selesai memodifikasi aturan sakelar tiket, mengubah limit jeda tunggu (*idle*), atau menggeser skala kreativitas, jangan lupa untuk menekan tombol hijau **Simpan** pada panel kanan **Simpan Perubahan** agar semua pengaturan tersimpan.