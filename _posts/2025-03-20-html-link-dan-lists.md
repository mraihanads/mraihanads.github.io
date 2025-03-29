---
layout : post
title : "HTML Link dan Lists"
---

Artikel ini membahas tentang tautan (link) dan daftar (lists) dalam HTML, yang merupakan elemen penting dalam pembuatan halaman web. Tautan digunakan untuk menghubungkan satu halaman dengan halaman lainnya, baik dalam situs yang sama maupun ke situs eksternal. Sementara itu, daftar digunakan untuk menyusun informasi dalam bentuk yang lebih terstruktur, seperti daftar berurutan (ordered list) dan daftar tak berurutan (unordered list).

![HTML Link dan Lists](/assets/images/gambar_html.png)

**HTML Link dan Lists** adalah dua fitur dasar dalam HTML yang digunakan untuk membuat halaman web lebih interaktif dan terorganisir. Berikut penjelasan singkatnya:

---

### **1. HTML Link**
HTML Link (atau hyperlink) adalah elemen yang memungkinkan pengguna untuk berpindah dari satu halaman web ke halaman lainnya atau ke bagian tertentu dalam halaman yang sama. Link dibuat menggunakan tag `<a>`.

#### Cara Kerja:
- **Tag `<a>`**: Digunakan untuk membuat link.
- **Atribut `href`**: Menentukan tujuan link (bisa berupa URL, file, atau ID elemen di halaman yang sama).
- **Teks atau Gambar**: Konten yang bisa diklik oleh pengguna.

#### Contoh:
```html
<a href="https://www.google.com">Kunjungi Google</a>
```
Ini akan menampilkan teks "Kunjungi Google" yang bisa diklik untuk membuka website Google.

---

### **2. HTML Lists**
HTML Lists digunakan untuk menampilkan informasi dalam bentuk daftar. Ada tiga jenis daftar dalam HTML:

#### a. **Unordered List (Daftar Tidak Berurutan)**
- Menggunakan bullet point (titik) untuk menandai setiap item.
- Dibuat dengan tag `<ul>` dan setiap item menggunakan tag `<li>`.

**Contoh:**
```html
<ul>
  <li>Apel</li>
  <li>Pisang</li>
  <li>Jeruk</li>
</ul>
```

Hasil:
- Apel
- Pisang
- Jeruk

---

#### b. **Ordered List (Daftar Berurutan)**
- Menggunakan nomor untuk menandai setiap item.
- Dibuat dengan tag `<ol>` dan setiap item menggunakan tag `<li>`.

**Contoh:**
```html
<ol>
  <li>Bangun tidur</li>
  <li>Mandi</li>
  <li>Sarapan</li>
</ol>
```
Hasil:
1. Bangun tidur
2. Mandi
3. Sarapan

---

#### c. **Description List (Daftar Deskripsi)**
- Digunakan untuk membuat daftar yang terdiri dari istilah (`<dt>`) dan deskripsinya (`<dd>`).
- Dibuat dengan tag `<dl>`.

**Contoh:**
```html
<dl>
  <dt>HTML</dt>
  <dd>Bahasa untuk membuat struktur halaman web.</dd>
  <dt>CSS</dt>
  <dd>Bahasa untuk mendesain tampilan halaman web.</dd>
</dl>
```
Hasil:
**HTML**  
Bahasa untuk membuat struktur halaman web.  
**CSS**  
Bahasa untuk mendesain tampilan halaman web.

---

### **Kesimpulan**
- **HTML Link** digunakan untuk menghubungkan halaman web atau bagian tertentu dalam halaman.
- **HTML Lists** digunakan untuk menyusun informasi dalam bentuk daftar, baik berurutan, tidak berurutan, atau deskriptif.
