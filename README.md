📝 Note App Flutter

Aplikasi catatan sederhana menggunakan Flutter dan SQLite sebagai penyimpanan database lokal.
Project ini dibuat untuk pembelajaran CRUD Flutter dengan implementasi:

✨ Dark Mode & Light Mode
🗂️ Penyimpanan data lokal SQLite
📝 Tambah, edit, hapus catatan
💾 Auto Save note
📱 UI sederhana dan responsive
🌙 Theme management
📸 Preview Aplikasi
🏠 Home Page
Menampilkan seluruh daftar catatan
Grid note card
Toggle dark/light mode
✍️ Detail Note
Tambah catatan
Edit catatan
Auto save saat kembali
Hapus catatan dengan dialog konfirmasi
🚀 Fitur Utama
🌙 Dark Mode & Light Mode

Aplikasi mendukung perubahan tema secara realtime menggunakan ThemeData.

theme: isDark ? AppTheme.dark : AppTheme.light
📝 CRUD Catatan

Fitur CRUD lengkap:

➕ Tambah catatan
✏️ Edit catatan
❌ Hapus catatan
📖 Lihat daftar catatan
💾 Database SQLite

Menggunakan package:

sqflite

Database lokal digunakan untuk menyimpan:

Judul catatan
Isi catatan
Author
Tanggal dibuat
Tanggal update
⚡ Auto Save

Ketika user menekan tombol kembali:

Navigator.pop(context, note);

data otomatis tersimpan ke SQLite.

🧱 Struktur Project
lib/
│
├── models/
│   └── note_model.dart
│
├── pages/
│   ├── home_page.dart
│   └── note_page.dart
│
├── services/
│   └── database_helper.dart
│
├── theme/
│   └── app_theme.dart
│
├── widgets/
│   ├── confirm_dialog.dart
│   └── note_card.dart
│
└── main.dart
🗃️ Struktur Database
Table: notes
Field	Type
id	INTEGER
title	TEXT
content	TEXT
author	TEXT
created_at	TEXT
updated_at	TEXT
📦 Dependencies

Tambahkan dependency berikut pada pubspec.yaml:

dependencies:
  flutter:
    sdk: flutter

  sqflite: ^2.4.2
  path: ^1.9.1
  google_fonts: ^6.2.1
⚙️ Install Project
1️⃣ Clone Repository
git clone https://github.com/username/noteapp.git
2️⃣ Masuk Folder Project
cd noteapp
3️⃣ Install Dependency
flutter pub get
4️⃣ Jalankan Aplikasi
flutter run
🧠 Teknologi Yang Digunakan
Teknologi	Fungsi
Flutter	Framework aplikasi
Dart	Bahasa pemrograman
SQLite	Database lokal
sqflite	Package SQLite Flutter
Google Fonts	Custom typography
📚 Materi Yang Dipelajari

Project ini cocok untuk pembelajaran:

StatefulWidget
Navigation
CRUD Flutter
SQLite Database
Theme Management
Dialog
Form Input
Local Storage
Clean Folder Structure
👨‍💻 Developer

Made with ❤️ using Flutter & SQLite.
