# 09. HTTP Services

Praktikum - Bagian 1: JSONPlaceHolder
---

* Membuka website http://jsonplaceholder.typicode.com/

![](img/09/1.bmp)

Praktikum - Bagian 2: Getting Data
---

* Membuat component baru dengan nama posts dengan perintah `ng g c posts`

![](img/09/2.bmp)

* Import HTTP Module pada file **app.module.ts**

![](img/09/3.bmp)

* Memodifikasi file **posts.component.ts** menjadi seperti berikut:

![](img/09/4.bmp)

* Memodifikasi file **posts.component.html** menjadi seperti berikut:

![](img/09/5.bmp)

* Hasilnya seperti berikut:

![](img/09/6.bmp)

* Meng-comment `HttpModule` pada file **app.module.ts**

![](img/09/7.bmp)

* Error akan muncul seperti berikut:

![](img/09/8.bmp)

> Penjelasan karena `HttpModule` dihapus, maka provider akan mencari http module

* Memperbaiki code pada file **posts.component.ts** menjadi seperti berikut:

![](img/09/9.bmp)

* Error akan muncul seperti berikut:

![](img/09/10.bmp)

> Penjelasan karena `HttpModule` dihapus, maka provider akan mencari http module

* Memodifikasi file **posts.component.html** menjadi seperti berikut:

![](img/09/11.bmp)

* Memodifikasi file **posts.component.ts** menjadi seperti berikut:

![](img/09/12.bmp)

* Hasilnya seperti berikut:

![](img/09/13.bmp)

Praktikum - Bagian 3: Creating Data
---

* Menambahkan code pada file **posts.component.html** menjadi seperti berikut:

![](img/09/14.bmp)

* Memodifikasi file **posts.component.ts** menjadi seperti berikut:

![](img/09/15.bmp)

* Hasilnya seperti berikut:

![](img/09/16.bmp)

Praktikum - Bagian 4: Updating Data
---

* Menambahkan code pada file **posts.component.ts** menjadi seperti berikut:

![](img/09/17.bmp)

* Menambahkan code pada file **posts.component.html** menjadi seperti berikut:

![](img/09/18.bmp)

* Hasilnya seperti berikut:

![](img/09/19.bmp)

> patch adalah untuk merequest http method

Praktikum - Bagian 5: Deleting Data
---

* Menambahkan code pada file **posts.component.ts** seperti berikut:

![](img/09/20.bmp)

* Menambahkan code pada file **posts.component.html** menjadi seperti berikut:

![](img/09/21.bmp)

* Hasilnya seperti berikut:

![](img/09/22.bmp)

> Menghapus element dari sebuah array dan, jika perlu, memasukkan element baru di tempat tersebut, mengembalikan element yang sudah dihapus.