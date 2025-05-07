---
layout : post
title : "Config.Yml"
---

Artikel ini membahas tentang file `config.yml`, yang sering digunakan dalam pengembangan website untuk menyimpan pengaturan konfigurasi. File ini biasanya digunakan dalam generator situs statis seperti Jekyll, Hugo, atau proyek berbasis YAML lainnya. `config.yml` membantu mengatur metadata, tema, plugin, dan variabel global yang diperlukan oleh website.

**Config.yml** adalah file konfigurasi berbasis YAML (*YAML Ain't Markup Language*) yang berisi pengaturan penting untuk proyek website. Berikut penjelasan singkatnya:

---

### **1. Apa Itu Config.yml?**
`config.yml` adalah file teks yang menggunakan sintaks YAML untuk menyimpan konfigurasi proyek. File ini mudah dibaca manusia (*human-readable*) dan sering digunakan untuk:  
- Mengatur judul, deskripsi, dan author website.  
- Menentukan tema atau plugin yang digunakan.  
- Menyimpan variabel global seperti URL, waktu build, atau pengaturan SEO.  

#### **Struktur Dasar YAML**  
YAML menggunakan indentasi (spasi/tab) untuk struktur data. Contoh:  
```yaml
title: Muhammad Raihan
description: Personal blog powered by Jekyll and GitHub Pages
author:  
  name: "Muhammad Raihan"  
  email: "mraihanads@gmail.com"  
```

---

### **2. Contoh Penggunaan Config.yml**  
Berikut contoh isi file `config.yml` dalam proyek Jekyll:  

```yaml
# Pengaturan Dasar  
title: "Muhammad Raihan"  
baseurl: ""  
url: "https://mraihanads.github.io"  

# Author  
author:  
  name: "Muhammad Raihan"  
  bio: "Penulis dan Developer"  

# Tema dan Plugin  
theme: minima  
plugins:  
  - jekyll-feed  
  - jekyll-seo-tag  

# Pengaturan Build  
timezone: Asia/Jakarta  
future: false  # Jangan tampilkan post dengan tanggal masa depan  
```

#### **Penjelasan:**  
- **`title` dan `url`**: Metadata dasar website.  
- **`author`**: Data penulis dengan sub-properti (`name`, `bio`).  
- **`theme` dan `plugins`**: Menentukan tema dan ekstensi yang digunakan.  
- **`timezone`**: Pengaturan lokalisasi waktu.  

---

### **3. Jenis Data dalam YAML**  
YAML mendukung berbagai tipe data:  

#### **a. String (Teks)**  
```yaml
nama: "Nilai String"  
```  

#### **b. Angka**  
```yaml
harga: 100  
```  

#### **c. Boolean**  
```yaml
draft: false  
```  

#### **d. List/Array**  
```yaml
kategori:  
  - HTML  
  - CSS  
  - JavaScript  
```  

#### **e. Objek**  
```yaml
social:  
  github: user123  
  twitter: handle123  
```  

---

### **4. Tips Penting**  
1. **Indentasi**: Gunakan spasi (bukan tab) untuk menghindari error.  
2. **Komentar**: Tambahkan komentar dengan `#` untuk penjelasan.  

---

### **Kesimpulan**  
- `config.yml` adalah file konfigurasi berbasis YAML yang fleksibel dan mudah dibaca.  
- Digunakan untuk menyimpan pengaturan website, tema, plugin, dan variabel global.  
- Sintaks YAML mengandalkan indentasi dan format *key-value*.  
