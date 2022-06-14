# Lab11Web

Nama    : Alif Fahmi
NIM     : 31201007
Kelas   : TI 20 B2

Latihan_11 1-6-2022

## Praktikum 11: PHP Framework (Codeigniter)

### Buat folder baru lab11_php_ci lalu Jalankan XAMPP Ubah file php.ini seperti berikut :

![ss 1](img/ss1-1.png)

![ss 1](img/ss1-2.png)

### Instal Codeigniter 4 simpan pada htdocs dan Buka http://localhost/lab11_php_ci/ci4/public/ , hasilnya :

![ss 1](img/ss2-1.png)

![ss 1](img/ss2-2.png)

### Buka cmd pada XAMPP Shell lalu buka php spark, untuk menjalankan server ketik "php spark serve" :

![ss 1](img/ss3-1.png)

Hasil error/kesalahan

![ss 1](img/ss3-2.png)

### Mengaktifkan mode Debugging dengan mengubah file .env menjadi = development, seperti berikut :

![ss 1](img/ss3-3.png)

### Untuk mencoba Error hilangkan tanda ; (titik koma) pada Home.php, seperti berikut :

![ss 1](img/ss4-1.png)

Contoh error/kesalahan akan ditampilkan secara detail

![ss 1](img/ss4-2.png)

### Mengarahkan router pada controller, kemudian Membuat Route Baru Tambahkan kode berikut pada Route.php :

![ss 1](img/ss5-1.png)

### Cek pada CMD dengan memasukan "php spark routes", Akses route yang telah dibuat dengan http://localhost:8080/about, hasilnya :

![ss 1](img/ss5-2.png)

![ss 1](img/ss5-3.png)

### Membuat Controller Page, dengan membuat file baru bernama page.php seperti berikut :

![ss 1](img/ss6-1.png)

Hasilnya :

![ss 1](img/ss6-2.png)

### Mengaktifkan AutoRouting dengan men set nilai true/false, jika true maka fungsi akan aktif

![ss 1](img/ss7-1.png)

### Tambahkan method baru pada Controller Page seperti berikut untuk page Term of Services

![ss 1](img/ss7-2.png)

Akses http://localhost:8080/page/tos hasilnya :

![ss 1](img/ss7-3.png)

### Membuat View, dengan membuat file baru bernama about.php dan masukan kode berikut :

![ss 1](img/ss8-1.png)

Ubah method about pada class Controller Page menjadi seperti berikut:

![ss 1](img/ss8-2.png)

Selanjutnya refresh Kembali browser

![ss 1](img/ss8-3.png)

### Membuat Layout Web dengan CSS
Buat file css pada direktori public dengan nama style.css

![ss 1](img/ss9-4.png)

Kemudian buat folder template pada direktori view kemudian buat file header.php dan footer.php

`header.php`

![ss 1](img/ss9-1.png)

`footer.php`

![ss 1](img/ss9-2.png)

Kemudian ubah file app/view/about.php seperti berikut

![ss 1](img/ss9-3.png)

Selanjutnya refresh tampilan pada alamat http://localhost:8080/about

![ss 1](img/ss9-5.png)

## Pertanyaan dan Tugas
Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.

Tambahkan kode berikut di dalam Routes.php

![ss 1](img/ss10-1.png)

edit page control pada page.php

![ss 1](img/ss10-2.png)

Buat file artikel.php dan contact.php pada direktori app/view/.....

![ss 1](img/ss10-3.png)

![ss 1](img/ss10-4.png)

saat kita membuka halaman artikel dan kontak maka tampilan akan menuju page artikel dan kontak

![ss 1](img/ss10-5.png)

![ss 1](img/ss10-6.png)

========================================================
## Praktikum 12: Framework Lanjutan (CRUD)

### Jalankan MySQL pada program XAMPP berjalan dan buat database seperti berikut :

![ss 1](img/ss11-1.PNG)

### Mengkonfigurasi koneksi database pada file .env seperti berikut :

![ss 1](img/ss11-2.PNG)

### Membuat file Model pada direktori app/Models dengan nama ArtikelModel.php seperti berikut :

![ss 1](img/ss11-3.PNG)

### Membuat file Controller baru dengan nama Artikel.php pada direktori app/Controllers. seperti berikut :

![ss 1](img/ss11-4.PNG)

### Membuat file Views baru dengan nama artikel pada direktori app/views, kemudian buat filebaru dengan nama index.php, seperti berikut 

![ss 1](img/ss12-1.PNG)

Jalankan server dan akses link : http://localhost:8080/artikel

![ss 1](img/ss12-2.PNG)

### Masukan data berikut pada database :

![ss 1](img/ss12-3.PNG)

Refresh dan lihat kembali browser :

![ss 1](img/ss12-4.PNG)

### Menambahkan Detail pada Artikel.php seperti berikut :

![ss 1](img/ss13.PNG)

### Membuat file baru baru untuk halaman detail dengan nama app/views/artikel/detail.php. seperti berikut :

![ss 1](img/ss13-1.PNG)

### Tambahkan rute baru pada Routes.php :

![ss 1](img/ss13-2.PNG)

Tampilan Artikel setelah di Klik :

![ss 1](img/ss13-3.PNG)

### Membuat Menu Admin

Buat method baru pada Controller Artikel dengan nama admin_index() :

![ss 1](img/ss14-1.PNG)

Buat file baru dengan nama admin_index.php pada folder artikel :

![ss 1](img/ss14-2.PNG)

Tambahkan Routing baru pada Routes.php seperti berikut :

![ss 1](img/ss14-3.PNG)

Akses menu admin dengan url http://localhost:8080/admin/artikel :

![ss 1](img/ss14-4.PNG)

### Menambah Data Artikel

Tambahkan fungsi/method baru pada Controller Artikel dengan nama add() :

![ss 1](img/ss15-1.PNG)

Lalu buat file baru dengan nama form_add.php pada folder artikel :

![ss 1](img/ss15-2.PNG)

tampilan saat klik artikel :

![ss 1](img/ss15-3.PNG)

### Mengubah DAta Artikel

Tambahkan fungsi/method baru pada Controller Artikel dengan nama edit() :

![ss 1](img/ss16-1.PNG)

Lalu buat file baru dengan nama edit_add.php pada folder artikel :

![ss 1](img/ss16-2.PNG)

Tampilan saat mengubah artikel :

![ss 1](img/ss16-3.PNG)

### Menghapus Data

Tambahkan fungsi/method baru pada Controller Artikel dengan nama delete() :

![ss 1](img/ss17-1.PNG)