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
![image](https://github.com/user-attachments/assets/df3fb2f9-2f66-455f-80d1-f29940e0fca9)


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
# 1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
   Jawab   
   Mengubah warna background color Di file style_eksternal.css  
   background awal
   ```sh
   #intro {
    background: #418fb1;
   ```
 ![Screenshot 2024-10-09 163535](https://github.com/user-attachments/assets/431ecbda-5a54-42c8-b51a-9a3e64bf13e3)

  Background setelah diubah
   ```sh
   #intro {
    background: #f331af;
   ```
  ![image](https://github.com/user-attachments/assets/fc46bbd0-bc1c-441c-bc30-eedf0aa3577e)

Menambahkan Border (Garis Pembatas)
Border awal(tidak ditambahkan ``border: 2px dashed #ff0000;``)
```sh
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
    }
```
![image](https://github.com/user-attachments/assets/2d40366e-47cb-46ad-85f1-b766fcedb84a)

Border setelah ditambahkan ``border: 2px dashed #ff0000;``
```sh
nav {
    background: #20A759;
    color:#fff;
    padding: 10px;
    border: 2px dashed #ff0000;
    }
```

![image](https://github.com/user-attachments/assets/522a1d29-8a85-4ee4-9fd0-12c25e8d95cf)

# 2. Apa perbedaan pendeklarasian CSS elemen ``h1 {...}`` dengan #intro ``h1 {...}``? berikan penjelasannya!   
Jawab   
Pendeklarasian ``h1{...}`` = adalah deklarasi umum yang menerapkan gaya pada semua elemen ``<h1>`` di halaman HTML. Semua elemen ``<h1>`` di seluruh halaman HTML akan mendapatkan gaya ini, tanpa memandang konteks atau di mana ``<h1>`` tersebut berada.  
Pendeklarasian ID: #intro ``h1 {...}`` = adalah deklarasi khusus yang hanya menerapkan gaya pada elemen ``<h1>`` di dalam elemen yang memiliki ID intro. Gaya ini hanya akan diterapkan pada elemen ``<h1>`` yang berada di dalam elemen dengan ID intro. Jika ada elemen ``<h1>`` di luar elemen #intro, gaya ini tidak berlaku.   
``h1 {...}`` berlaku untuk semua elemen ``<h1>`` di seluruh halaman.   
#intro ``h1 {...}`` hanya berlaku untuk elemen ``<h1>`` yang ada di dalam elemen dengan ID intro.   

# 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!   
Jawab   
Mengubah dibagian inline CSS
```sh
<h1 style="color: orange; font-size: 30px;">CSS Internal dan <i>Inline CSS</h1>
```
![image](https://github.com/user-attachments/assets/1c5d278b-349d-4244-acfa-7fc7f21743fb)

Mengubah dibagian CSS eksternal
```sh
nav {
    background: #000080; 
    color: #ffffff;
    padding: 15px;
    border: 3px solid #0000ff; 
}
```
![image](https://github.com/user-attachments/assets/6269f96a-932f-44ed-9186-cc197b8dc738)

Mengubah dibagian CSS internal
```sh
 h1 {
    font-size: 24px;
    color: #0F189F;
    text-align: center;
    padding: 20px 10px;
     }
```
(tidak berubah karena inline CSS meng override.)   
Untuk elemen ``<h1>``, warna dan ukuran font akan mengikuti inline CSS (color: orange; font-size: 30px;), karena ini memiliki prioritas tertinggi dibandingkan internal atau eksternal CSS.   
Untuk elemen nav, browser akan mengikuti CSS eksternal, sehingga perubahan background: #000080 dan border: 3px solid #0000ff akan diterapkan.  
Jadi, Jika gaya di CSS eksternal tidak memiliki konflik dengan gaya di CSS internal atau inline, maka keduanya bisa diterapkan, Misalnya, jika CSS internal mendeklarasikan gaya untuk elemen ``<h1>`` dan tidak ada inline style yang menimpa, maka gaya CSS eksternal juga tidak akan mempengaruhi elemen ``<h1>`` .   

# 5. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ``( <p id="paragraf-1" class="text-paragraf"> )``
Jawab   
Elemen HTML
```sh
<p id="paragraf-1" class="text-paragraf">Paragraf dengan ID dan Class.</p>
```
CSS di internal
```sh
#paragraf-1 {
    color: blue; 
}

.text-paragraf {
    color: red; 
}
```
![image](https://github.com/user-attachments/assets/a2fb12c4-c6a7-45c0-b429-215745f08210)   
jadi, gaya yang ditampilkan browser adalah declaration dari ID   
Gaya untuk ID (color: blue;) memiliki spesifisitas yang lebih tinggi dibandingkan dengan gaya untuk Class (color: red;). Karena ID memiliki spesifisitas yang lebih tinggi, maka warna teks yang akan ditampilkan di browser adalah biru, meskipun ada gaya untuk kelas yang mendeklarasikan warna merah. Jika ada dua atau lebih deklarasi CSS yang berkonflik pada elemen yang sama, yang memiliki ID dan Class, maka declaration dari ID yang akan ditampilkan pada browser karena ID memiliki prioritas lebih tinggi dibandingkan Class dalam spesifisitas CSS.







