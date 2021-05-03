Sebelum membuka Web API ini dibutuhkan :

1. Webserver seperti xampp, wampp dan lain-lain
2. Kontak.zip yang ada di dalam repository

Setelah semua yang dibutuhkan sudah siap, extract Kontak.zip tersebut 
sampai muncul dua folder yaitu rest_ci sebagai server dan rest_ci_client sebagai client.

Setelah itu, pindahkan kedua folder itu ke dalam htdocs pada direktori xampp atau webserver yang kalian gunakan.

Di xampp, di bagian apache dan my sql tekan bagian start agar bisa membuat database terlebih dahulu

Di platform website yang kalian gunakan ketik : localhost/phpmyadmin

Kemudian ke bagian import dan import file telepon.sql


Untuk membuka web API tersebut, ketik di platform website yang kalian gunakan :
http://127.0.0.1/rest_ci_client/index.php/kontak

Kegunaan dari Web API ini :

1. Dapat menambah data kontak
2. Dapat merubah data kontak
3. Dapat menghapus data kontak
