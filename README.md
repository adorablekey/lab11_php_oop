# lab11_php_oop
# NAMA : KEYSIA NURHAYATI BR PANJAITAN
# NIM  : 31410350
# KELAS  : TI 24 A4

# persiapan struktur folde
      lab11_php_oop/
      │── .htaccess
      │── config.php
      │── index.php
      │── class/
      │    ├── Database.php
      │    └── Form.php
      │── module/
      │    └── artikel/
      │         ├── index.php
      │         ├── tambah.php
      │         └── ubah.php
      └── template/
           ├── header.php
           ├── footer.php
           └── sidebar.php

Tujuan struktur ini:
 untuk Memisahkan layout, class, konfigurasi, dan modul supaya coding lebih rapi.

 # Penjelasan File Penting
# A. File Database.php
Merupakan class OOP untuk menyambungkan PHP ke MySQL.

Fungsinya meliputi:
koneksi database

query

insert

update

get data

Dengan class ini, kamu tidak perlu query manual di tiap file.

# B. File Form.php
Class OOP untuk membuat form input dinamis.

Fungsi yang disediakan:

addField() → menambah input

displayForm() → menampilkan form otomatis

Mendukung:

text

textarea

select

radio

checkbox

password

Tujuan:

Agar form dibuat otomatis melalui OOP, bukan manual.

# File config.php

Berisi konfigurasi database:

            $config = [
                'host' => 'localhost',
                'username' => 'root',
                'password' => '',
                'db_name' => 'latihan_oop'
            ];
Class Database akan membaca file ini.

# File .htaccess

Fungsi utamanya:

Mengaktifkan URL Routing

Tanpa .htaccess:

localhost/lab11_php_oop/index.php?module=artikel&page=tambah


Dengan .htaccess:

localhost/lab11_php_oop/artikel/tambah


Lebih rapi seperti framework Laravel.

# File index.php

Ini adalah router utama (mirip controller pusat).

Tugasnya:

Membaca URL
Contoh: /artikel/tambah

Memecah menjadi:

modul = artikel

page = tambah

Mencari file:
module/artikel/tambah.php

Load layout (header, sidebar, footer)

Jadi index.php adalah "gerbang" utama.

4. Cara Kerja Routing

Misal kamu akses:

       localhost/lab11_php_oop/artikel/index

Maka router akan menjalankan:

module/artikel/index.php


Jika kamu buka:

      localhost/lab11_php_oop/artikel/tambah

Maka file yang dipanggil:

module/artikel/tambah.php


Jika file tidak ada → muncul pesan Modul Tidak Ditemukan.

# Pembuatan Modul (Contoh: Artikel)

Folder:

module/artikel/


Isinya:

index.php → menampilkan list data artikel

tambah.php → form tambah artikel

ubah.php → form edit artikel

Semua file bisa memakai class:

Database

Form

Jadi coding lebih mudah dan rapi.

<img width="1920" height="1200" alt="Screenshot 2025-12-11 141208" src="https://github.com/user-attachments/assets/cc86f501-4264-4fbc-a18e-95a32889db50" />

<img width="1920" height="1200" alt="Screenshot 2025-12-11 141242" src="https://github.com/user-attachments/assets/0f11a646-7c3e-4dd9-9fb0-fbbaf9f2aac9" />

<img width="1920" height="1200" alt="Screenshot 2025-12-11 141320" src="https://github.com/user-attachments/assets/66104bf0-a87b-40ae-8ba8-a4a675ddbe40" />


