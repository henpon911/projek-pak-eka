# Prompt Pembuatan Database MySQL

Salin prompt berikut ke AI untuk membuat skrip database MySQL yang cocok dengan aplikasi ini.

```text
Bertindaklah sebagai database engineer. Buatkan skrip SQL MySQL 8 untuk aplikasi Student Management REST API berbasis Express.js.

Spesifikasi aplikasi:
- Nama database: db_toko
- Nama tabel: siswa
- Backend menghubungkan MySQL lokal dengan konfigurasi host localhost, user root, dan password kosong.
- Endpoint API membaca dan menulis kolom: id, nis, nama, kelas, jurusan, alamat.
- id digunakan sebagai primary key dan nilainya dibuat otomatis.
- nis adalah nomor induk siswa.
- nama, kelas, jurusan, dan alamat menyimpan data teks.
- Aplikasi mengirim nilai nis, nama, kelas, jurusan, dan alamat saat membuat atau mengubah data siswa.

Buat output berupa:
1. Skrip SQL lengkap yang bisa dijalankan dari awal, termasuk CREATE DATABASE dan CREATE TABLE.
2. Tipe data yang sesuai, primary key, AUTO_INCREMENT, dan aturan NOT NULL untuk data wajib.
3. Character set dan collation yang mendukung teks Bahasa Indonesia, gunakan utf8mb4.
4. Beberapa INSERT contoh dengan data fiktif yang aman untuk pengujian.
5. SELECT untuk memeriksa tabel dan data setelah skrip dijalankan.
6. Instruksi singkat menjalankan skrip melalui MySQL CLI atau phpMyAdmin.

Pastikan nama database, tabel, dan kolom persis sama dengan spesifikasi agar kompatibel dengan routes/siswa.js. Jangan mengubah struktur API atau menambahkan kolom wajib yang tidak disebutkan. Gunakan placeholder data contoh, bukan data pribadi nyata. Jelaskan apabila memilih batas panjang kolom atau constraint tambahan.
```

## Catatan

Konfigurasi backend saat ini menunjuk ke database `db_toko`. Kredensial koneksi untuk penggunaan lokal berada di `routes/siswa.js`. Jangan gunakan konfigurasi user `root` tanpa password untuk lingkungan produksi.
