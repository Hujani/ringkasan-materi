Ringkasan BAB 1 & BAB 2 — Modul Praktikum Basis Data

BAB 1 — Review Konversi ER Diagram ke Skema Relasi



Tujuan Pembelajaran

Memahami cara mengonversi ER Diagram menjadi skema relasi dan tabel fisik.

Memudahkan proses transformasi dari level view (ERD) ke level fisik database.


Materi Utama

1. Aturan Konversi ERD → Relasi → Tabel

Entitas kuat menjadi satu tabel, atribut menjadi kolom, PK sebagai primary key.

Composite attribute dipecah menjadi kolom masing-masing.

Multivalue attribute menjadi tabel baru.

Derived attribute dapat dibuat kolom biasa.

Entitas lemah: PK entitas kuat menjadi FK pada tabel entitas lemah.

Relasi 1–1: salah satu tabel membawa FK.

Relasi 1–N: pihak N menyimpan FK.

Relasi M–N: dibuat tabel baru berisi FK dari kedua tabel.

Unary, ternary, generalisasi–spesialisasi, dan agregasi memiliki aturan konversi tersendiri.



2. Studi Kasus Skema Pembayaran Apotik

ERD apotek dikonversikan menjadi 13 tabel, antara lain:
PASIEN, RESEP, OBAT, PEGAWAI, PEMBAYARAN, DETAIL_OBAT, dll.





---

BAB 2 — Pengantar Basis Data & DDL



Tujuan Pembelajaran

Mengenal dasar-dasar database dan DBMS.

Memahami MySQL, instalasi, cara akses, tipe data, serta dasar penggunaan DDL.


Materi Utama

1. Konsep Dasar Database

Database adalah kumpulan tabel yang saling terhubung.

DBMS adalah sistem untuk mengelola database, contoh: MySQL, Oracle, PostgreSQL.



2. MySQL

DBMS yang menggunakan SQL, bersifat open-source, cepat, reliable, dan multiplatform.



3. Instalasi MySQL

Disarankan menggunakan XAMPP (membawa MySQL/MariaDB + phpMyAdmin).



4. Mengakses MySQL

Via command prompt menggunakan:

mysql -u root -p

Menutup MySQL: \q



5. Tipe Data MySQL

INT, FLOAT, DATE, DATETIME, CHAR, VARCHAR, BLOB, dll.



6. DDL (Data Definition Language)

Perintah untuk membuat dan mengelola struktur database.

Membuat database

CREATE DATABASE nama_db;

Melihat database

SHOW DATABASES;

Menggunakan database

USE nama_db;

Menghapus database

DROP DATABASE nama_db;


