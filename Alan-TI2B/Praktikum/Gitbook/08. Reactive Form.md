# 08. Reactive Form

Praktikum - Bagian 1: Building a Bootstrap Form
---

* Membuat component baru dengan nama `signup-form` dengan perintah sebagai berikut:

![](img/08/1.bmp)

* Memodifikasi **app.component.html** menjadi seperti berikut:

![](img/08/2.bmp)

* Memodifikasi filr **signup-form.component.html** menjadi seperti berikut:

![](img/08/3.bmp)

* Hasilnya seperti berikut:

![](img/08/4.bmp)

Praktikum - Bagian 2: Control Programmatically
---

* Memodifikasi file **sign-up-form.component.ts** seperti berikut:

![](img/08/5.bmp)

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/6.bmp)

* Maka akan muncul error seperti berikut:

![](img/08/7.bmp)

* Memodifikasi file **app.module.ts** seperti berikut:

![](img/08/8.bmp)

Praktikum - Bagian 3: Adding Validation
---

* Memodifikasi file **signup-form.component.ts** menjadi seperti berikut:

![](img/08/9.bmp)

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/10.bmp)

* Hasilnya seperti berikut:

![](img/08/11.bmp)

* Menambahkan `get username` pada file **signup-form.component.ts** seperti berikut:

```typescript
  get username() {
    return this.form.get('username');
  }
```

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/12.bmp)

* Hasilnya seperti berikut:

![](img/08/13.bmp)

Praktikum - Bagian 4: Specific Validation Errors
---

* Memodifikasi file **signup-form.component.ts** menjadi seperti berikut:

![](img/08/14.bmp)

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/15.bmp)

* Hasilnya seperti berikut:

![](img/08/16.bmp)

Praktikum - Bagian 5: Custome Validation
---

* Membuat file baru pada folder `signup-form` dengan nama **username.validators.ts** kemudian isi dengan script sebagai berikut:

![](img/08/17.bmp)

* Memodifikasi file **signup-form.component.ts** menjadi seperti berikut:

![](img/08/18.bmp)

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/19.bmp)

* Hasilnya seperti berikut:

![](img/08/20.bmp)

Praktikum - Bagian 6: Asyncronus Validation
---

* Memodifikasi file **username.validators.ts** menjadi seperti berikut:

![](img/08/21.bmp)

* Memodifikasi file **signup-form.component.ts** menjadi seperti berikut:

![](img/08/22.bmp)

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/23.bmp)

* Hasilnya seperti berikut:

![](img/08/24.bmp)

Praktikum - Bagian 7: Displaying a Loader Image
---

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/25.bmp)

* Hasilnya seperti berikut:

![](img/08/26.bmp)

Praktikum - Bagian 8: Validating Form on Submit

* Memodifikasi file **signup-form.component.ts** menjadi seperti berikut:

```typescript
  login() {
    this.form.setErrors({
      invalidLogin: true
    });
  }
```

* Memodifikasi file **sign-up-form.component.html** seperti berikut:

![](img/08/27.bmp)

* Hasilnya seperti berikut:

![](img/08/28.bmp)