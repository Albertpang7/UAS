Sebelum membuka Web API ini dibutuhkan :

1. Webserver seperti xampp, wampp dan lain-lain
2. Kontak.zip yang ada di dalam repository

Setelah semua yang dibutuhkan sudah siap, extract Kontak.zip tersebut 
sampai muncul dua folder yaitu rest_ci sebagai server dan rest_ci_client sebagai client.

Setelah itu, pindahkan kedua folder itu ke dalam htdocs pada direktori xampp atau webserver yang kalian gunakan.

Di xampp, di bagian apache dan my sql tekan bagian start agar bisa membuat database terlebih dahulu
Di platform website yang kalian gunakan ketik : localhost/phpmyadmin

Setelah masuk, di bagian bawah ada bagian console ketikan :
```html
CREATE DATABASE kontak;
```
baru control + enter untuk eksekusi

Setelah itu ketik lagi :
```html
USE kontak;
CREATE TABLE IF NOT EXISTS `telepon` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `nama` varchar(50) NOT NULL,
  `nomor` varchar(13) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=latin1 AUTO_INCREMENT=8 ;
```
baru control + enter 

Terakhir :
```html
USE kontak;
INSERT INTO `telepon` (`id`, `nama`, `nomor`) VALUES
(1, 'Brody', '08576666792'),
(2, 'Thamuz', '08576666791'),
(3, 'Layla', '08576666743');
```
baru control + enter

Untuk membuka web API tersebut, ketik di platform website yang kalian gunakan :
http://127.0.0.1/rest_ci_client/index.php/kontak

Kegunaan dari Web API ini :

1. Dapat menambah data kontak
2. Dapat merubah data kontak
3. Dapat menghapus data kontak
