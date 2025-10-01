# Modul Praktikum Pemrograman Web
Nama : ANDREAN PUTRA ARYA

Nim : 312410341

Kelas : TI.24.A4

# Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat file baru dengan nama lat2web1.html
3. Buat struktur dasar dari dokumen HTML.
4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.

# 1. Membuat Dokumen HTML
Buatlah dokumen HTML seperti berikut :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar Pemula</title>
</head>
<body>
    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>
    <nav>
        <a href="lab2_css_dasar.html">CSS Basic</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>

    <div id="intro">
        <h1>Hello World</h1>
        <p>SAYA <b>ANDREAN PUTRA ARYA</b> DENGAN NIM <b>312410341</b> kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di 
        <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat 
        tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>

        <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
    </div>
</body>
</html>
```
Selanjutnya buka pada brwoser untuk melihat hasilnya :

![gambar](https://github.com/andreanbadeh/Lab2html-cssweb1/blob/225f956797ccd09ec2b6212052733d50dffa1c43/image/Screenshot%20from%202025-10-01%2018-59-40.png)

# 2. Mendeklarasikan CSS Internal
Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
  <style>
    body {
      font-family: 'Open Sans', sans-serif;
    }
    header {
      min-height: 80px;
      border-bottom: 1px solid #77CCEF;
    }
    h1 {
      font-size: 24px;
      color: #0F189F;
      text-align: center;
      padding: 20px 10px;
    }
    h1 i {
      color: #6d6a6b;
    }
  </style>
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>
  
  <nav>
    <a href="lab2_css_dasar.html">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>

  <div id="intro">
    <h1>Hello World</h1>
    <p>
      SAYA <b>ANDREAN PUTRA ARYA</b> DENGAN NIM <b>312410341</b> kami sedang belajar HTML dan CSS dasar, 
      pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. 
      Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal 
      tag-tag dasar HTML dan CSS.
    </p>

    <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
  </div>
</body>
</html>
```
Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat hasilnya.

![gambar](https://github.com/andreanbadeh/Lab2html-cssweb1/blob/0187f14a21f2224c35f4ec4d2c9d398504114359/image/Screenshot%20from%202025-10-01%2019-06-51.png)

# 3. Menambahkan Inline CSS
Kemudian tambahkan deklarasi inline CSS pada tag p seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>CSS Dasar</title>
  <style>
    body {
      font-family: 'Open Sans', sans-serif;
    }
    header {
      min-height: 80px;
      border-bottom: 1px solid #77CCEF;
    }
    h1 {
      font-size: 24px;
      color: #0F189F;
      text-align: center;
      padding: 20px 10px;
    }
    h1 i {
      color: #6d6a6b;
    }

    #intro p {
      text-align: center;
      color: #ccd8e4;
      line-height: 1.6;
    }
    nav a {
      margin-right: 15px;
      text-decoration: none;
      color: #0F189F;
    }
    nav a:hover {
      color: #77CCEF;
    }
  </style>
</head>
<body>
  <header>
    <h1>CSS Internal dan <i>Inline CSS</i></h1>
  </header>
  
  <nav>
    <a href="lab2_css_dasar.html">CSS Dasar</a>
    <a href="lab2_css_eksternal.html">CSS Eksternal</a>
    <a href="lab1_tag_dasar.html">HTML Dasar</a>
  </nav>

  <div id="intro">
    <h1>Hello World</h1>
    <p>
      SAYA <b>ANDREAN PUTRA ARYA</b> DENGAN NIM <b>312410341</b> kami sedang belajar HTML dan CSS dasar, 
      pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. 
      Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal 
      tag-tag dasar HTML dan CSS.
    </p>

    <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
  </div>
</body>
</html>
```

Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![gambar](https://github.com/andreanbadeh/Lab2html-cssweb1/blob/1e21efc923ae1e26c01508ea355718f5b64fd8ea/image/Screenshot%20from%202025-10-01%2019-15-57.png)

# 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css kemudian buatlah deklarasi CSS seperti berikut.
Kalau internal CSS ditulis di dalam file HTML, Eksternal CSS dipisahin jadi file khusus dengan ekstensi .css. Jadi HTML sama CSS tidak bercampur, lebih mudah kalo nanti mau edit tampilan.
Bikin file baru di folder project, kasih nama lat2web1.css 
Kemudian buat kode seperti yang ada di contoh pratikum
```
nav {
  background: #20A759;
  color: #fff;
  padding: 10px;
}

nav a {
  color: #fff;
  text-decoration: none;
  padding: 10px 20px;
}

nav .active,
nav a:hover {
  background: #0B6B3A;
}
```

Sekarang buka file lat2web1.html tadi, Tambahin tag di dalam buat nyambungin ke file CSS eksternal

![gambar](

Tampilan hasil nya :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab2Web/efa1dfd75127e85f51816f5a26d359c9560cbd15/Cuplikan%20layar%202025-09-30%20232532.png)

# 5. Menambahkan CSS Selector
Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file style_eksternal.css, tambahkan kode berikut.

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab2Web/52723fc9af873b28999bf536a8a13831595bb1b4/Cuplikan%20layar%202025-09-30%20233856.png)

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab2Web/52723fc9af873b28999bf536a8a13831595bb1b4/Cuplikan%20layar%202025-09-30%20233835.png)
