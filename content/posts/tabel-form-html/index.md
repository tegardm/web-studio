---
title       : "Tabel dan Form dalam HTML (Pertemuan 2)"
date            : 2024-05-07
description : "Menurut (Kustiyahningsih & Anamisa, 2011) HTML (Hypertext Markup
Languange) adalah standar bahasa yang digunakan untuk menampilkan dokumen
web. Sebuah dokumen HTML sendiri adalah dokumen teks yang dapat diedit oleh
editor teks apapun."
tags        : [ html, "tabel","form","input" ]
toc         : true
---

## Pengenalan Tabel HTML

Dalam pembuatan halaman web, tabel adalah salah satu elemen yang sangat penting. Tabel digunakan untuk menampilkan data secara terstruktur dan terorganisir. Dalam HTML, tabel dibuat menggunakan tag-tag tertentu yang memungkinkan penataan data dalam bentuk baris dan kolom.

### Struktur Dasar Tabel HTML

Tabel HTML terdiri dari beberapa elemen dasar, yaitu:

1. `<table>`: Tag ini digunakan untuk mendefinisikan sebuah tabel.
2. `<tr>`: Tag ini digunakan untuk mendefinisikan sebuah baris dalam tabel.
3. `<td>`: Tag ini digunakan untuk mendefinisikan sebuah sel dalam tabel (data cell).
4. `<th>`: Tag ini digunakan untuk mendefinisikan sebuah sel header dalam tabel (header cell).

Berikut adalah contoh struktur dasar sebuah tabel HTML:

```html
<table border="1">
  <tr>
    <th>Nama</th>
    <th>Usia</th>
  </tr>
  <tr>
    <td>John</td>
    <td>30</td>
  </tr>
  <tr>
    <td>Jane</td>
    <td>25</td>
  </tr>
</table>
```

### Penjelasan Mengenai Setiap Elemen Tabel

1. **`<table>`**: Ini adalah tag pembuka dan penutup untuk mengawali dan mengakhiri sebuah tabel dalam HTML. Semua elemen tabel, seperti baris dan sel, harus berada di antara tag ini.

2. **`<tr>`**: Ini adalah singkatan dari "table row" atau baris tabel. Setiap baris dalam tabel HTML didefinisikan oleh tag ini. 

3. **`<td>`**: Singkatan dari "table data", tag ini mendefinisikan sebuah sel atau cell yang berisi data dalam tabel. 

4. **`<th>`**: Singkatan dari "table header", tag ini digunakan untuk mendefinisikan sel header dalam tabel. Biasanya digunakan untuk menandai judul atau nama kolom.

### Atribut Tabel

Dalam contoh sebelumnya, ada atribut `border="1"` yang ditambahkan ke tag `<table>`. Atribut ini digunakan untuk menentukan lebar garis batas tabel. Anda juga bisa menambahkan atribut lain seperti `width`, `height`, `bgcolor`, dan lainnya untuk mengatur penampilan tabel.

### Penggunaan Tabel dalam Praktik

Tabel dalam HTML tidak hanya digunakan untuk menampilkan data berupa teks. Mereka juga dapat digunakan untuk menampilkan gambar, hyperlink, dan bahkan elemen-elemen HTML lainnya dalam setiap sel. Misalnya, Anda bisa menyisipkan gambar atau tautan di dalam sel tabel untuk membuat tata letak halaman web menjadi lebih menarik dan informatif.

### Responsifitas dan Desain Tabel

Dalam desain modern halaman web, penting untuk memperhatikan responsifitas tabel, terutama ketika diakses melalui perangkat seluler. Anda dapat menggunakan CSS untuk mengatur ulang tata letak tabel agar lebih responsif, misalnya dengan menggunakan media queries untuk menyesuaikan tampilan tabel sesuai dengan lebar layar perangkat.

Dengan memahami dasar-dasar pembuatan tabel dalam HTML dan penerapannya dalam desain web, Anda dapat membuat halaman web yang lebih terstruktur dan informatif bagi pengguna.


## Penggunaan HTML Form

Form merupakan salah satu elemen penting dalam HTML yang digunakan untuk mengumpulkan data dari pengguna melalui halaman web. Dengan menggunakan form, pengguna dapat mengirimkan informasi seperti teks, angka, pilihan, dan lainnya ke server untuk diproses.

### Struktur Dasar Form HTML

Form dalam HTML didefinisikan menggunakan tag `<form>`. Di dalam tag `<form>`, Anda dapat menempatkan berbagai elemen input, seperti teks box, tombol radio, kotak centang, dan lainnya.

Contoh struktur dasar form HTML:

```html
<form action="/proses" method="post">
  <label for="nama">Nama:</label>
  <input type="text" id="nama" name="nama"><br><br>
  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br><br>
  <input type="submit" value="Submit">
</form>
```

### Elemen Input

Ada beberapa jenis elemen input yang dapat digunakan dalam sebuah form, di antaranya:

- **Text Input**: Digunakan untuk mengumpulkan input teks dari pengguna.
- **Email Input**: Digunakan untuk mengumpulkan alamat email.
- **Password Input**: Digunakan untuk mengumpulkan kata sandi.
- **Checkbox**: Digunakan untuk memilih satu atau beberapa pilihan dari daftar.
- **Radio Button**: Digunakan untuk memilih satu pilihan dari beberapa pilihan.
- **Select Box**: Digunakan untuk memilih satu pilihan dari daftar drop-down.

Contoh penggunaan elemen input:

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username"><br><br>

<label for="password">Password:</label>
<input type="password" id="password" name="password"><br><br>

<label for="email">Email:</label>
<input type="email" id="email" name="email"><br><br>

<input type="checkbox" id="agree" name="agree" value="agree">
<label for="agree">Saya setuju dengan syarat dan ketentuan</label><br><br>

<input type="radio" id="male" name="gender" value="male">
<label for="male">Laki-laki</label><br>

<input type="radio" id="female" name="gender" value="female">
<label for="female">Perempuan</label><br><br>

<label for="cars">Pilih mobil:</label>
<select id="cars" name="cars">
  <option value="volvo">Volvo</option>
  <option value="saab">Saab</option>
  <option value="fiat">Fiat</option>
  <option value="audi">Audi</option>
</select><br><br>
```

### Atribut Form

Ada beberapa atribut yang dapat ditambahkan ke tag `<form>`, di antaranya:

- **action**: Menentukan URL tempat data form akan dikirim. Misalnya, jika Anda ingin data form dikirim ke halaman `proses.php`, Anda dapat menentukan `action="/proses.php"`.
- **method**: Menentukan metode pengiriman data, seperti "get" atau "post". Metode "get" akan mengirimkan data form sebagai query string di URL, sedangkan metode "post" akan menyembunyikan data form dari URL.
- **enctype**: Menentukan jenis encoding data sebelum dikirimkan ke server. Biasanya digunakan saat Anda ingin mengirimkan file dalam form. Nilai yang umum digunakan adalah `multipart/form-data`.

Contoh penggunaan atribut form:

```html
<form action="/proses" method="post" enctype="multipart/form-data">
  <!-- Isi form di sini -->
</form>
```
***
Coba Kode Diatas Melalu Codepen  :
[Buka Codepan](https://codepen.io/pen/)
