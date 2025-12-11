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
