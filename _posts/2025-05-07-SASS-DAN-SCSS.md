---
layout: post
title: "Mengenal SASS dan SCSS"
---

Pembahasan tentang **SASS** dan **SCSS**, yang merupakan preprocessor CSS modern. Preprocessor ini digunakan untuk menulis CSS dengan cara yang lebih efisien, terstruktur, dan mudah dipelihara. Dengan SASS dan SCSS, pengembang web dapat menggunakan fitur seperti variabel, nesting (aturan bersarang), mixin, pewarisan, dan lainnya yang tidak tersedia dalam CSS biasa.


**SASS dan SCSS** membantu mempercepat pengembangan front-end dengan menambahkan kemampuan pemrograman ke dalam penulisan stylesheet. Berikut penjelasan singkatnya:

---

### **1. Apa Itu SASS dan SCSS**

**SASS** (Syntactically Awesome Stylesheets) adalah preprocessor CSS yang memungkinkan kita menulis CSS dengan fitur tambahan seperti variabel, fungsi, nesting, dan lain-lain.

**SCSS** adalah versi baru dari SASS yang menggunakan sintaks mirip CSS, menjadikannya lebih familiar dan populer di kalangan developer.

#### Perbedaan SASS dan SCSS

| Fitur                 | `.sass` (SASS)                     | `.scss` (SCSS)                    |
|----------------------|------------------------------------|-----------------------------------|
| Gaya penulisan       | Tanpa `{}` dan `;` (indentasi)     | Menggunakan `{}` dan `;` seperti CSS |
| Kompatibel dengan CSS| Tidak                              | Ya                                |
| Digunakan saat ini   | Kurang populer                     | Lebih umum digunakan              |


---

### **2. Fitur-Fitur SCSS / SASS**

#### a. **Variabel**

Kita bisa menyimpan nilai (warna, ukuran, dsb) dalam sebuah variabel untuk digunakan berulang kali.

```scss
$primary-color: #3498db;

body {
  background-color: $primary-color;
}

```

---

#### b. **Nesting (Aturan Bersarang)**
Kita bisa menulis kode CSS di dalam selector lain, mirip dengan struktur HTML.

```scss
nav {
  ul {
    list-style: none;
  }

  li {
    display: inline-block;
  }

  a {
    text-decoration: none;
  }
}
```
---

#### c. **Operasi Matematika**
SCSS juga mendukung operasi matematika langsung di dalam kode.

```scss
.container {
  width: 100% / 3;
}
```

---