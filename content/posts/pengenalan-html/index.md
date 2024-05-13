---
title       : "Pengenalan HTML (Pertemuan 1)"
date            : 2024-05-07
description : "Menurut (Kustiyahningsih & Anamisa, 2011) HTML (Hypertext Markup
Languange) adalah standar bahasa yang digunakan untuk menampilkan dokumen
web. Sebuah dokumen HTML sendiri adalah dokumen teks yang dapat diedit oleh
editor teks apapun."
tags        : [ html, "fundamental","introduction" ]
toc         : true
---

## Pengertian HTML
Menurut (Kustiyahningsih & Anamisa, 2011) HTML (Hypertext Markup
Languange) adalah standar bahasa yang digunakan untuk menampilkan dokumen
web. Sebuah dokumen HTML sendiri adalah dokumen teks yang dapat diedit oleh
editor teks apapun. 

Dokumen HTML punya beberapa elemen yang dikelilingi oleh
tag-teks yang dimulai dengan symbol < dan berakhir dengan sebuah symbol > .
Editor teks yang penyusun gunakan adalah Notepad++ dan Xampp versi 1.8.
untuk web servernya menggunkaan bahasa pemrograman PHP

## Struktur Dasar HTML
Elemen HTML dimulai dengan tag awal, yang diikuti dengan isi elemen dan
tag akhir. Tag berakhir termasuksimbol / diikuti oleh tipe elemen, misalnya
`</head>` Sebuah elemen HTML dapat bersarang di dalam elemen lainnya.
Sebuah dokumen HTML standar terlihat seperti ini :

```HTML
<html>
  <head>
    <title>Judul Halaman Web</title>
  </head>
  <body>
    Percobaan Pertama
  </body>
</html>
```
Keterangan :
1. Tag HTML secara default dimulai dari `<HTML>` dan diakhiri dengan
`</HTML>`.
2. Tag `<HEAD> … </HEAD>` merupakan tag kepala sebelum badan. Tag
kepala ini akan terlebih dulu dieksekusi sebelum tag badan. Di dalam tag ini
berisi tag `<META>` dan `<TITLE>`. Tag `<META>` merupakan informasi atau
header suatu dokumen HTML. Atribut yang dimiliki oleh tag ini antara lain :
    * HTTP_EQUIV, atribut ini berfungsi untuk menampilkan dokumen HTML
    secara otomatis dalam jangka waktu tertentu.
    * CONTENT, atribut ini berisi informasi tentang isi document HTML yang
    akan dipanggil.
    * NAME, atribut ini merupakan identifikasi dari meta itu sendiri. Tag
      `<META>` dalam suatu document HTML boleh ada maupun tidak. 
3. Tag `<TITLE> … </TITLE>` adalah tag judul. Sebaiknya setiap halaman web
memiliki judul, dan judul tersebut dituliskan di dalam `<TITLE> …</TITLE>`. 
Judul ini akan muncul dalam titlebar dari browser.
4. Tag `<BODY> … </BODY>` adalah tag berisi content dari suatu halaman
web.

## Contoh Penggunaan Script HTML
{{< img "html1.png" "Contoh penggunaan script di HTML." border >}}
Keterangan :

**Contoh 1** : Judul Web

**Halo apa kabar?**

**Mudah-mudahan kabarnya baik-baik saja** : Merupakan perintah yang di buat
diantara `<body>` dan `</body>`.

Kemudian simpan file di atas di dalam folder c:\XAMPP\htdocs\ buat folder baru
untuk menyimpan file di dalam folder htdocs dalam contoh ini buat folder
webprog. Simpan file dengan nama contoh1.php didalam folder tersebut.
Pembuatan nama file pada saat penyimpanan harus diakhiri dengan extention
“.php”.

Buka browser (Google chrome, Mozilla etc) untuk membuka tampilan laman web
html yang telah kita buat tersebut. Ketikan di url: localhost/webprog
Maka akan tampil sebagai berikut:
{{< img "html2.png" "Contoh penggunaan script di HTML." border >}}
Kode-kode dalam HTML biasanya disebut TAG. Tag adalah sesuatu yang
digunakan untuk menandai elemen-elemen dalam suatu dokumen HTML. Tag
dalam HTML terdiri dari tanda lebih kecil ( < ), tanda lebih besar ( > ), dan garis
miring ( / ). Biasanya Tag dituliskan secara berpasangan, misanya `<h1>` dan
`</h1>`. Tag yang tidak menggunakan garis miring ( / ) adalah Tag pembuka atau
awal elemen. Sedangkan yang Tag yang mengandung garis miring ( / ) adalah
penutup elemen atau akhir elemen. Namun, ada juga Tag yang dalam
pemakaiannya tidak berpasangan, diantaranya adalah :
1. Tag untuk ganti paragraph yaitu <p>
2. Tag untuk ganti baris atau line break yaitu <br> 
3. Tag untuk garis datar yaitu <hr>
4. Tag list item yaitu <li> 

## Beberapa Contoh Tag HTML Lainnya
Kategori|Tag HTML|Keterangan/Kegunaan
---|---|---|
Basic|`<br>`|Memasukan Satu Baris Putus
Basic|`<hr>`|Tag Untuk Membuat Sebuah Garis Pemisah Untuk Dua Bagian
Formatting|`<blockquote>`| Tag untuk membuat text atau menandai bahwa dikutip dari sumber lain
Formatting|`<center>`| Tag untuk membuat text simeteris di posisikan di tengah
Forms|`<form>`|Tag untuk membuat form HTML untuk input pengguna
Forms|`<input>`|Tag untuk membuat sebuah kontrol input
Frames|`<iframe>`|Tag untuk membuat sebuah bingkai
Frames|`<frameset>`|Tag untuk membuat satu set bingkai (tidak disupport HTML5)
Images|`<img>`|Tag untuk memungkinkan menambahkan gambar
Images|`<map>`|Tag untuk memasukan informasi peta
Audio/Video|`<audio>`|Tag untuk menambahkan media audio
Audio/Video|`<source>`|Tag untuk menambahkan media audio/video lebih dalam HTML
Links|`<a>`|Tag untuk membuat hyperlink
Links|`<nav>`|Tag untuk membuat navigasi link
List|`<ul>`|Tag untuk membuat list tidak berurut
List|`<ol>`|Tag untuk membuat list yang berurut
Tables|`<table>`|Tag untuk membuat tabel di HTML
Tables|`<caption>`|Tag untuk membuat caption tabel di HTML

Dalam HTML sendiri penggunaan Tag disesuaikan dengan kebutuhan pembuatan
tampilan web nya, masih banyak Tag-tag HTML yang tidak peulis sebutkan disini,
tapi bisa langsung di praktekan pada script hTML nantinya
Contoh script HTML menggunakan Tag :
{{< img "html3.png" "Contoh penggunaan script HTML dengan tag." border >}}
Hasilnya :
{{< img "html4.png" "Contoh penggunaan script HTML dengan tag." border >}}

---

Coba Kode Diatas Melalu Codepen  :
[Buka Codepan](https://codepen.io/pen/)

