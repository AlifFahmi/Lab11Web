# Lab11Web
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