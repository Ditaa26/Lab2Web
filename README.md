# Lab2Web
Dita Tiara Putri (312310131)

# 1. Membuat dokumen HTML
``` sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
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
        <!-- CSS ID Selector -->
        <div id="intro">
             <h1>Hello World</h1>
             <p>Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman
                Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat
                adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
             <!-- CSS Class Selector -->
             <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
        </div>
</body>
</html>
```
![image](https://github.com/user-attachments/assets/3f8a2e91-4457-46f2-b08b-30b686d06089)

# 2. Mendeklarasikan CSS Internal
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
    <style>
        body {
        font-family:'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom:1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color:#6d6a6b;
        }
        </style>
</head>
```
![image](https://github.com/user-attachments/assets/cccd17bc-00f0-4520-8ea2-ed8dfeecb159)

# 3. Menambahkan Inline CSS   
```sh
  <div id="intro">
             <h1>Hello World</h1>
             <p style="text-align: center; color: #ccd8e4;">
                Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.</p>
             <!-- CSS Class Selector -->
             <a class="button btn-primary" href="#intro">Informasi selengkapnya.</a>
        </div>
```
![image](https://github.com/user-attachments/assets/4b709678-e489-4f27-a841-e7f44a35c2b7)

# 4. Membuat CSS Eksternal
Buatlah file baru dengan nama style_eksternal.css   
![image](https://github.com/user-attachments/assets/71416b68-1087-401c-9ea2-4c79065bf3f4)
```sh
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
    }
    nav a {
    color: #fff;
    text-decoration: none;
    padding:10px 20px;
    }
    nav .active,
    nav a:hover {
    background: #0B6B3A;
    }
```
Kemudian tambahkan tag <link> untuk merujuk file css yang sudah dibuat pada bagian ``<head>``
```sh
<!DOCTYPE html>
<html lang="en">
<head>
    <!-- menyisipkan css eksternal -->
<link rel="stylesheet" href="style_eksternal.css" type="text/css">
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
    <style>
        body {
        font-family:'Open Sans', sans-serif;
        }
        header {
            min-height: 80px;
            border-bottom:1px solid #77CCEF;
        }
        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }
        h1 i {
            color:#6d6a6b;
        }
        </style>
</head>
```

# 5. Menambahkan CSS Selector  
Selanjutnya menambahkan CSS Selector Menggunakan ID dan Class Selector pada file style_eksternal.css
```sh
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
    }
    #intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
    }
    /* Class Selector */
    .button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
    }
    .btn-primary {
    background: #E42A42;
    }
```
![image](https://github.com/user-attachments/assets/c7b3d430-08c2-46e6-a935-960302370cb1)

# Pertanyaan dan Tugas  
1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.   
2. Apa perbedaan pendeklarasian CSS elemen ``h1 {...}`` dengan #intro ``h1 {...}``? berikan penjelasannya!   
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!   
4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ``( <p id="paragraf-1" class="text-paragraf"> )``







