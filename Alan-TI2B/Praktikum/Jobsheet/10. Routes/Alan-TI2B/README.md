# 10. Routes

Praktikum - Bagian 1: Configure the Routes
---

* Membuat komponen posts, form-member, navbar, not-found, dan home

![](img/10/1.bmp)

* Buka file **app.module.ts**. Memastikan komponen pada langkah 1 sudah terdaftar seperti berikut:

![](img/10/2.bmp)

* Menambahkan module router pada file **app.module.ts** seperti berikut:

![](img/10/3.bmp)

* Buka file **navbar.component.html** kemudian menambahkan code sebagai berikut:

![](img/10/4.bmp)

* Buka file **navbar.component.html** kemudian ganti code menjadi sebagai berikut:

![](img/10/5.bmp)

* Hasilnya seperti berikut:

![](img/10/6.bmp)

Praktikum - Bagian 2: Router Outlet
---

* Buka file **app.component.html** kemudian menambahkan code sebagai berikut:

![](img/10/7.bmp)

* Hasilnya seperti berikut:

![](img/10/8.bmp)

* Inspect Element:

![](img/10/9.bmp)

> app-navbar berhasil di jalankan

* Menjalankan link **localhost:4200/form** 

![](img/10/10.bmp)

* Menjalankan link **localhost:4200/post** 

![](img/10/11.bmp)

* Menjalankan link **localhost:4200/coba** 

![](img/10/12.bmp)

> Penjelasan langkah 3, 4 dan 5: Membuat beberapa outlet untuk link. Setiap link mempunyai component sendiri kecuali link **localhost:4200/coba** karena tidak dibuatkan component

Praktikum - Bagian 3: Add Link
---

* Buka file **navbar.component.html** kemudian menambahkan link pada href tiap menu seperti berikut:

![](img/10/13.bmp)

> Jika klik navbar home dan post, maka link akan berubah menjadi .../home dan .../post

* Memodifikasi href menjadi routerLink pada halaman **navbar.component.html** seperti berikut:

![](img/10/14.bmp)

* Hasilnya seperti berikut:

![](img/10/15.bmp)

* Memodifikasi class li pada file **navbar.component.html** menjadi seperti berikut:

![](img/10/16.bmp)

* Hasilnya seperti berikut:

![](img/10/17.bmp)

Praktikum - Bagian 4: Accessing Route Parameter
---

* Membuat komponen baru bernama **profile** dengan perintah `ng g c profile`

![](img/10/18.bmp)

* Buka file **app.module.ts** kemudian menambahkan route untuk profile sebagai berikut:

![](img/10/19.bmp)

* Buka file **home.component.html** kemudian menambahkan code sebagai berikut:

![](img/10/20.bmp)

* Modifikasi file **profile.component.ts** menjadi seperti berikut:

![](img/10/21.bmp)

* Hasilnya seperti berikut:

![](img/10/22.bmp)

> Link Joko Bowo mempunyai id, yang terletak pada routerLink

* Modifikasi file **profile.component.ts** menjadi seperti berikut:

![](img/10/23.bmp)

* Hasilnya seperti berikut:

![](img/10/24.bmp)