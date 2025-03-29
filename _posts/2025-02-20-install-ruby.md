---
layout : post
title : "Install Ruby dan Jekyll"
---

artikel ini menjelaskan cara Install Ruby dan Jekyll

### 1. Kebutuhan Aplikasi dan Tools

- **Sistem Operasi:** *Windows*, *Linux*, atau *macOS*
- **Integrated Development Environment:** Visual Studio Code
- **Web Browser:** Google Chrome
- **GitHub:** Web-based version control repository.
- **Markdown** untuk menulis laporan.
- **Git** sebagai version control.
- **Ruby dan Jekyll** untuk membuat halaman web statis.

**Note :**
Kebutuhan aplikasi dan tool dapat disesuaikan dengan speksifikasi atau kondisi di laptop masing-masing.

---

### 2. Instalasi

Beberapa kebutuhan aplikasi dan tools diatas perlu diinstall seperti Ruby, Git, Google Chrome dan Visual Studio Code.

a. Install Ruby dan Jekyll
- Ruby versi 2.7.0 atau yang lebih tinggi, **ruby -v**.
- RubyGems, **gem -v**
- GCC dan Make, **gcc -v** **g++ -v** dan **make -v**
- Download Ruby Installer melalui link berikut [Ruby Installer](https://rubyinstaller.org/downloads)
- Ikuti form instalsi Ruby Installer.

b. Install Git
- Download Git Installer melalui link [Git Installer](https://git-scm.com/downloads) 
- Pilih sesuai dengan sistem operasi yang digunakan, misla Windows.  
- Pada bagian Standalone Installer pilih yang 64 bit.  

c. Install Visual Studio Code  
- Download VSCode Installer melalui link [VSCode Installer](https://code.visualstudio.com/download)
- Pilih sesuai dengan sistem operasi yang digunakan, misla Windows.  
- Pada bagian System Installer pilih yang 64 bit (x64).  

d. Install Google Chrome  
- Download Google Chrome Installer melalui link Google Chrome Installer.  
- Klik tomboh Download Chrome.

---

### 3. Personal Web dengan Jekyll dan GitHub Page

Untuk membuat personal web dengan Jekyll dan publish di GitHub Page ikuti langkahlangkah berikut ini:
- Buat akun di GitHub dengan username sesuai nama masing-masing.
- Buat repository baru dengan nama username dan github.io.
  Contoh: username github = faiza, maka nama repositorya faiza.github.io.
- Clone repository tersebut ke lokal.
- Masuk ke dalam folder repository tersebut kemudian install Jekyll dengan perintah berikut melalui terminal.

---

```text
┌───────────────────────────────┐
│  *Terminal*                   |
|  gem install jekyll bundler   |
└───────────────────────────────┘
```
---

- Jalankan perintah bundle init untuk inisialisasi folder tersebut sebagai proyek jekyll seperti perintah berikut ini. Hasil dari perintah tersebut adalah file baru dengan nama Gemfile.

---

```text
┌───────────────────────────────┐
│  *Terminal*                   |
|  bundle init                  |
└───────────────────────────────┘
```
--- 

- Edit file Gemfile menggunakan IDE dan tambahkan kode berikut.

---

```text
┌───────────────────────────────┐
│  *IDE*                        |
|  gem "jekyll"                 |
└───────────────────────────────┘
```
---

- Buat file baru dengan nama index.html, kemudian isi dengan kode berikut.

---

```text
┌───────────────────────────────┐
|*IDE*                          |
|<!DOCTYPE html>                |
|<html>                         |
|<head>                         |
|    <meta charset="utf-8">     |
|    <title>Home</title>        |
|</head>                        |
|<body>                         |
|    <h1>Hello World!</h1>      |
|</body>                        |
|</html>                        |
└───────────────────────────────┘
```
---

- Jalankan jekyll build untuk build web yang telah dibuat sehingga menhasilkan directory_site.

---
```text
┌───────────────────────────────┐
│  *Terminal*                   |
|  jekyll build                 |
└───────────────────────────────┘
```
---

- Kemudian jalankan perintah jekyll serve untuk menjalankan web yang telah dibuat di web browser dengan alamat http://localhost:4000.

---

```text
┌───────────────────────────────┐
│  *Terminal*                   |
|  jekyll serve                 |
└───────────────────────────────┘
```
---

- Jika web telah berhasil dibuka, edit file **Gemfile.lock** dengan menambahkan platform linux pada bagian platform seperti pada gambar berikut.

---

```text
┌───────────────────────────────┐
│  *IDE*                        |
|  PLATFORMS                    |
|  x86_64-linux                 |
└───────────────────────────────┘
```
---

- Selanjutnya push repositori ke GitHub dengan perintah-perintah berikut.

---

```text
┌────────────────────────────────────┐
│  *Terminal*                        |
|  jekyll serve git add .            |
|  git commit -m "pub: First publish"|
|  git push                          |
└────────────────────────────────────┘
```
---

- Buat GitHub Actions untuk CI/CD agar web otomatis publish.

---

**Note:**

Ketika menjalankan jekyll dalam tahap pengembangan, gunakan perintah jekyll serve –livereload agar ketika ada perubahan web browser langsung menampilkan hasil perubahannya. Apabila dalam menjalankan jekyll terjadi error karena port konflik jalankan menggunakan –host dan –port.
