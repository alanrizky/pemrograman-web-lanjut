# 03. Angular Fundamental

Praktikum - Bagian 1: Component Basic
---

* Membuat komponen dengan nama **courses** dengan cara ` ng g c courses `.
![](img/03/1.bmp)

* Kemudian ke directory **src/app** kemudian buka file **app.component.html**.
* Edit isi file tersebut menjadi seperti berikut:

```html
<app-courses></app-courses>

<router-outlet></router-outlet>
```

* Kemudian jalankan menggunakan ` ng serve --open `

![](img/03/2.bmp)

* Buka file **app.modules.ts** dan hapus ` coursecomponent ` pada ` declarations `.

![](img/03/3.bmp)

* Jalankan angular.
* Terdapat error bahwa **app-courses** merupakan elemen yang tidak diketahui.

![](img/03/4.bmp)

> **Penjelasan**: ` CoursesComponent ` merupakan elemen penting pada **NgModule**, jika dihapus maka angular tidak dapat menampilkan isi dari html.

Praktikum - Bagian 2: Templates
---

* Pindah direktori ke **../courses**.
* Buka file **courses.component.ts** kemudian tambahkan property baru dengan nama **title**.

![](img/03/5.bmp)

* Kemudian tambahankan string pada binding datanya. Buka file **courses.component.html**, dan tambahkan code seperti berikut:

```html
<p>
  courses works!
</p>
<p>
  {{"judulnya:" + title}}
</p>
```
* Hasilnya seperti berikut:

![](img/03/6.bmp)

* Buka file **courses.component.ts** dan buat sebuah method dengan nama ` getTitle ` seperti berikut:

![](img/03/7.bmp)

* Ubah code pada file **courses.component.html** seperti berikut:

![](img/03/9.bmp)

* Hasilnya seperti berikut:

![](img/03/8.bmp)

Praktikum - Bagian 3: Directive
---

* Buka file **courses.component.ts** dan membuat property dengan nama **course** dengan data berupa array. Seperti berikut:

```typescript
import { Component, OnInit } from '@angular/core';

@Component({
  selector: 'app-courses',
  templateUrl: './courses.component.html',
  styleUrls: ['./courses.component.css']
})
export class CoursesComponent implements OnInit {

  title = 'Belajar Angular';
  Title() {
    return this.title;
  }
  Courses = [
    {id: 0, name: 'HTML'},
    {id: 1, name: 'PHP'},
    {id: 2, name: 'ANGULAR'},
    {id: 3, name: 'C#'},
    {id: 4, name: 'VB.NET'}
  ]

  constructor() { }

  ngOnInit() {
  }

}
```

* Buka file **courses.component.html** lalu ditambahkan directive ` ngFor ` dan string interpolation seperti berikut:

![](img/03/10.bmp)

* Hasil pada browser:

![](img/03/11.bmp)

Praktikum - Bagian 4: Services dan Dependency Injection
---

* Membuat service baru yang bernama **courses** dengan perintah ` ng g s courses `.

![](img/03/12.bmp)

* Buka file **courses.service.ts** kemudian ditambahkan method getCourse seperti berikut:

![](img/03/13.bmp)

* Kemudian memodifikasi file **courses.component.ts** seperti berikut:

```typescript
import { Component, OnInit } from '@angular/core';

@Component({
  selector: 'app-courses',
  templateUrl: './courses.component.html',
  styleUrls: ['./courses.component.css']
})
export class CoursesComponent implements OnInit {

  title = 'Belajar Angular';
  Title() {
    return this.title;
  }
  Courses;

  constructor() { }

  ngOnInit() {
  }

}
```

* Hasilnya seperti berikut:

![](img/03/14.bmp)

* Menambahkan constructor seperti berikut:

```typescript
import { Component, OnInit } from '@angular/core';
import { CoursesService } from '../courses.service';

@Component({
  selector: 'app-courses',
  templateUrl: './courses.component.html',
  styleUrls: ['./courses.component.css']
})
export class CoursesComponent implements OnInit {

  title = 'Belajar Angular';
  Title() {
    return this.title;
  }
  Courses;

  constructor(private service:CoursesService) { 
    this.Courses = service.getCourses;
  }

  ngOnInit() {
  }

}
```

* Hasilnya seperti berikut:

![](img/03/14.bmp)
