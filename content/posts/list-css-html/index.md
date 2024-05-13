---
title       : "Tentang List dan CSS di HTML (Pertemuan 3)"
date            : 2024-05-07
description : "Materi ini akan membahas tentang penggunaan list dalam HTML, termasuk Ordered List (OL), Unordered List (UL), dan List Item (LI)."
tags        : [html, list, css, style, ordinal]
toc         : true
---

## Penggunaan List dalam HTML

List merupakan salah satu elemen penting dalam HTML yang digunakan untuk menampilkan informasi secara terstruktur. Terdapat dua jenis utama list dalam HTML, yaitu Ordered List (OL) dan Unordered List (UL). Setiap item dalam list didefinisikan menggunakan List Item (LI).

### Ordered List (OL)

Ordered List digunakan untuk membuat daftar yang memiliki urutan atau nomor. Setiap item dalam Ordered List diberi nomor atau angka secara otomatis.

Contoh penggunaan Ordered List:

```html
<ol>
  <li>Pertama</li>
  <li>Kedua</li>
  <li>Ketiga</li>
</ol>
```
### Unordered List (UL)
Unordered List digunakan untuk membuat daftar yang tidak memiliki urutan tertentu. Setiap item dalam Unordered List ditandai dengan simbol bullet atau titik.

Contoh penggunaan Unordered List:
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
### List Item (LI)
List Item digunakan untuk mendefinisikan setiap item dalam sebuah list, baik itu dalam Ordered List maupun Unordered List.

Contoh penggunaan List Item:
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>

<ol>
  <li>Pertama</li>
  <li>Kedua</li>
  <li>Ketiga</li>
</ol>
```

### List Bersarang

Dalam HTML, Anda dapat menyusun list bersarang, yaitu list yang memiliki hierarki atau tingkat kedalaman. Ini berguna ketika Anda perlu menyajikan informasi yang lebih terstruktur. Anda dapat menyisipkan list di dalam list, baik itu dalam Ordered List maupun Unordered List.

Contoh penggunaan list bersarang:

```html
<ul>
  <li>Pertama</li>
  <li>Kedua
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Ketiga</li>
</ul>

<ol>
  <li>Pertama</li>
  <li>Kedua
    <ol>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ol>
  </li>
  <li>Ketiga</li>
</ol>
```


## Penggunaan CSS di HTML

CSS (Cascading Style Sheets) digunakan untuk mengatur tampilan dan gaya halaman web, seperti warna, ukuran font, tata letak, dan dekorasi. CSS dapat diterapkan pada elemen HTML menggunakan beberapa metode, seperti inline, internal, dan eksternal.

### Metode Inline CSS

Metode ini melibatkan penggunaan atribut `style` di dalam tag HTML. Inline CSS didefinisikan langsung pada elemen HTML tertentu.

Contoh penggunaan Inline CSS:

```html
<p style="color: blue; font-size: 16px;">Ini adalah teks dengan gaya inline CSS.</p>
```


CSS (Cascading Style Sheets) digunakan untuk mengatur tampilan dan gaya halaman web, seperti warna, ukuran font, tata letak, dan dekorasi. CSS dapat diterapkan pada elemen HTML menggunakan beberapa metode, seperti inline, internal, dan eksternal.

### Metode Inline CSS

Metode ini melibatkan penggunaan atribut `style` di dalam tag HTML. Inline CSS didefinisikan langsung pada elemen HTML tertentu.

Contoh penggunaan Inline CSS:

```html
<p style="color: blue; font-size: 16px;">Ini adalah teks dengan gaya inline CSS.</p>
```

### Metode Internal CSS
Metode ini melibatkan penempatan kode CSS di dalam tag <style> di dalam bagian <head> dokumen HTML.

Contoh penggunaan Internal CSS :
```html
<!DOCTYPE html>
<html>
<head>
  <title>Halaman dengan Internal CSS</title>
  <style>
    p {
      color: green;
      font-size: 18px;
    }
  </style>
</head>
<body>
  <p>Ini adalah teks dengan gaya internal CSS.</p>
</body>
</html>
```

### Metode Eksternal CSS
Metode ini melibatkan penulisan kode CSS dalam file terpisah dengan ekstensi .css, dan kemudian file tersebut dihubungkan dengan dokumen HTML menggunakan tag `<link>` di dalam bagian `<head>`.
Contoh penggunaan Eksternal CSS:
```html
<!DOCTYPE html>
<html>
<head>
  <title>Halaman dengan Eksternal CSS</title>
  <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  <p>Ini adalah teks dengan gaya eksternal CSS.</p>
</body>
</html>
```

### Keuntungan Penggunaan CSS
Penggunaan CSS memisahkan struktur (HTML) dari tampilan (CSS), sehingga memudahkan pemeliharaan dan pengembangan halaman web. Dengan CSS, Anda dapat dengan mudah mengubah tampilan seluruh situs web hanya dengan mengedit satu file CSS.

Dengan memahami penggunaan CSS di HTML, Anda dapat membuat halaman web yang lebih menarik dan mudah dikelola.
***
Coba Kode Diatas Melalu Codepen  :
[Buka Codepan](https://codepen.io/pen/)