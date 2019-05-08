# 11. Authentication and Authorization

Praktikum - Bagian 1: Implementation Login
---

* Membuka folder **auth-demo-starter**

![](img/11/1.bmp)

* Menginstall angular2-jwt dengan perintah `npm install angular2-jwt --save`:

![](img/11/2.bmp)

* Hasilnya seperti berikut:

![](img/11/3.bmp)

* Membuka file **auth.service.ts** kemudian menambahkan code seperti berikut:

![](img/11/4.bmp)

* Mengisi email dan password pada login.

![](img/11/5.bmp)

* Mengisi email dengan format yang salah

![](img/11/6.bmp)

* Membuka file **auth.service.ts** kemudian ganti code menjadi sebagai berikut:

![](img/11/7.bmp)

* Hasilnya seperti berikut:

![](img/11/8.bmp)

Praktikum - Bagian 2: Implementasi Logout
---

* Membuka file **home.component.html** kemudian menambahkan code seperti berikut:

![](img/11/9.bmp)

* Membuka file **auth.service.ts** kemudian menambahkan code seperti berikut:

![](img/11/10.bmp)

* Hasilnya seperti berikut:

![](img/11/11.bmp)

Praktikum - Bagian 3: Getting the Current User
---

* Membuat token di jwt.io

![](img/11/12.bmp)

* Membuka file **auth.service.ts** kemudian ganti code menjadi sebagai berikut:

![](img/11/13.bmp)

* Membuka file **auth.service.ts** kemudian menambahkan code seperti berikut:

![](img/11/14.bmp)

* Membuka file **auth.service.ts** kemudian ganti token menjadi berikut:

![](img/11/15.bmp)

* Membuka file **home.component.html** kemudian ganti code menjadi sebagai berikut:

![](img/11/16.bmp)

* Halaman awal

![](img/11/17.bmp)

* Login seperti yang sudah di tentukan

![](img/11/18.bmp)

* Token akan tersimpan

![](img/11/19.bmp)

* Nama akan berubah sesuai login

![](img/11/20.bmp)

* Halaman admin

![](img/11/21.bmp)

* Logout maka token akan hilang

![](img/11/22.bmp)

> Penjelasan : Kita masuk sebagai admin (token yang sudah dibuat adalah user sebagai admin), jadi jika kita login, dengan user itu, maka halaman admin akan terbuka. Dan jika di logout maka token akan hilang.