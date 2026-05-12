# aplikasi_data_telpon

<div align="center">
  <img width="522" height="1078" alt="Screenshot 2026-05-12 132756" src="https://github.com/user-attachments/assets/35d08056-2fdf-4c2f-8f3d-37ed283735ec" />
<img width="523" height="1078" alt="Screenshot 2026-05-12 132809" src="https://github.com/user-attachments/assets/47df7cbc-612e-43ff-b76f-06655f67ba06" />
<img width="516" height="1078" alt="Screenshot 2026-05-12 132818" src="https://github.com/user-attachments/assets/233c2d60-1193-44bc-9c5c-db3071cca988" />
<img width="510" height="1078" alt="Screenshot 2026-05-12 132825" src="https://github.com/user-attachments/assets/40302621-187c-41bf-97f5-ebd044e625ee" />
</div>

A new Flutter project.

## Deskirpsi Project
aplikasi_data_nelpon adalah aplikasi penyimpanan data nomor telepon sederhana berbasis Flutter menggunakan SQLite sebagai database lokal.

Aplikasi ini digunakan untuk:
Menyimpan nomor telepon
Menampilkan daftar kontak
Mengedit data kontak
Menghapus kontak
Menyimpan data secara offline

Project ini dibuat untuk mempelajari konsep CRUD (Create, Read, Update, Delete) menggunakan Flutter dan SQLite.

✨ Fitur Aplikasi
➕ Menambahkan data telepon
✏️ Mengedit data
❌ Menghapus data
📋 Menampilkan daftar nomor telepon
💾 Penyimpanan lokal SQLite
📱 Tampilan sederhana dan ringan
🛠️ Teknologi yang Digunakan
Teknologi	Fungsi
Flutter	Framework aplikasi
Dart	Bahasa pemrograman
SQLite	Database lokal
sqflite	Package SQLite Flutter
path	Mengatur lokasi database
path_provider	Mengambil direktori penyimpanan
📂 Struktur Folder
lib/
│
├── models/
│   └── contact_model.dart
│
├── pages/
│   ├── add_contact_page.dart
│   └── home_page.dart
│
├── services/
│   └── database_helper.dart
│
├── widgets/
│   ├── contact_card.dart
│   └── confirm_dialog.dart
│
└── main.dart

📖 Penjelasan Struktur Folder
📁 models
Berisi model data aplikasi.

contact_model.dart
Digunakan untuk membuat struktur data kontak.

Contoh data:
id
nama
nomor telepon

📁 pages
Berisi halaman utama aplikasi.

home_page.dart
Halaman utama untuk menampilkan semua data nomor telepon.

Fitur:
menampilkan daftar kontak
tombol tambah data
tombol edit
tombol hapus

add_contact_page.dart
Halaman untuk menambahkan atau mengedit data telepon.

Fitur:
input nama
input nomor telepon
simpan data

📁 services
Berisi logic database SQLite.

database_helper.dart
Digunakan untuk:
membuat database
insert data
read data
update data
delete data

📁 widgets
Berisi widget reusable.

contact_card.dart
Widget card untuk menampilkan data kontak.

confirm_dialog.dart
Dialog konfirmasi hapus data.

📄 main.dart
File utama aplikasi Flutter.

Fungsi:
menjalankan aplikasi
menentukan halaman pertama
konfigurasi MaterialApp
🗃️ Database SQLite

Aplikasi menggunakan SQLite sebagai database lokal.
Nama tabel:
contacts

Struktur tabel:
Kolom	Tipe
id	INTEGER
name	TEXT
phone	TEXT
📦 Package yang Digunakan

Tambahkan package berikut pada pubspec.yaml

dependencies:
  flutter:
    sdk: flutter

  sqflite: ^2.3.0
  path: ^1.9.0
  path_provider: ^2.1.2

Install package:

flutter pub get
🔄 Konsep CRUD
1️⃣ Create

Menambahkan data kontak baru.

await db.insert("contacts", data);
2️⃣ Read

Mengambil semua data kontak.

await db.query("contacts");
3️⃣ Update

Mengubah data kontak.

await db.update("contacts", data);
4️⃣ Delete

Menghapus data kontak.

await db.delete("contacts");
▶️ Cara Menjalankan Project

Clone repository:

git clone https://github.com/username/aplikasi_data_nelpon.git

Masuk ke folder project:

cd aplikasi_data_nelpon

Jalankan aplikasi:

flutter run
📱 Tampilan Aplikasi
🏠 Home Page

Menampilkan daftar data nomor telepon.

Fitur:

list data kontak
tombol edit
tombol hapus
tombol tambah data
➕ Add Contact Page

Halaman input data nomor telepon.

Fitur:

input nama
input nomor telepon
simpan data
🚀 Pengembangan Selanjutnya

Fitur yang dapat ditambahkan:

🔍 Search kontak
⭐ Favorite kontak
📷 Foto profil kontak
☁️ Backup cloud
🌙 Dark mode
📞 Direct call
📌 Kesimpulan

Project aplikasi_data_nelpon merupakan aplikasi CRUD sederhana berbasis Flutter dan SQLite yang digunakan untuk menyimpan data nomor telepon secara offline.

Project ini cocok untuk belajar:

Flutter dasar
SQLite database
CRUD
Stateful Widget
Navigasi halaman
Reusable widget

Aplikasi ini juga dapat dikembangkan menjadi aplikasi kontak yang lebih lengkap di masa depan.
