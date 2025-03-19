# mvc-example
1. setelah clone jangan lupa update composer use "composer update"

Pada versi ini, digunakan style psr4 untuk autoloading.

Dalam contoh ini tidak ada routing controller melalui address bar, melainkan menggunakan query browser biasa.

Untuk tabel-nya dapat dibuat terlebih dahulu menggunakan database mysql,

CREATE TABLE mahasiswa (id int(11) not null auto_increment primary key, nim char(14) not null, nama varchar(255) not null) -> copy dan paste ke jendela query mysql
tambahkan atribut pada database table mahasiswa yaitu create_at, delete_at, is-delete. 

Create_at = untuk menyimpan data waktu ketika data dimasukan ke database,
Delete_at = untuk menyimpan data waktu ketika dihapus soft delete,
Is_delete = disini saya menggunakan tin, jika data baru buat makan default 0, dan 1 untuk digunakan soft delete

Untuk koneksi database, saya menggunakan PDO sebagai pengganti dari mysql_connect() info lengkap, kunjungi http://php.net/manual/en/book.pdo.php
