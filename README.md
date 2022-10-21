# Latihan Membuat CSS Layout pada website

* Nama          : Hizbullah Ridwan
* NIM           : 312110055
* Kelas         : TI.21.B.1
* Mata Kuliah   : Pemrograman Web

Dalam latihan Membuat CSS Layout ini, saya menggunakan [Google Chrome](https://www.google.com/intl/id_id/chrome/) sebagai web browser dan [visual studio code](https://code.visualstudio.com/) sebagai teks editornya.       

## Membuat Box Element

Pertama adalah membuat box elementnya terlebih dahulu, tambahkan tag `<section>` kemudian didalamnya         
tambahkan tag `<div>`.                

```bash
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Box Element</title>
    </head>
    <body>
        <header>
            <h1>Box Element</h1>
        </header>
        <section>
            <div class="div1">Div 1</div>
            <div class="div2">Div 2</div>
            <div class="div3">Div 3</div>
        </section>
    </body>
</html>
```         

## CSS Float Property

CSS float property ditambahkan didalam CSS. Untuk itu maka harus ditambahkan terlebih dahulu tag CSS nya       
dengan cara tambahkan tag `<style>`. Kemudian didalamnya ditambahkan `float:left` supaya box element div        
berada diposisi sebelah kiri.          

```bash
<style>
div {
    float:left;
    padding: 10px;
}
.div1 {
    background: red;
}
.div2 {
    background: yellow;
}
.div3 {
    background: green;
}
</style>
```         

![Gambar 1](Screenshoots/Capture1.PNG)       

## Mengatur Clearfix Element

Sebelum membuat sebuah clearfix element, tambahkan terlebih dahulu `div` berikutnya dan bisa dibilang sebagai div 4.          
Tambahkan juga classnya yaitu `div4` supaya CSS nya bisa diatur. Tambahkan `clear:left` di CSS.      

```bash
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```     

![Gambar 2](Screenshoots/Capture2.PNG)        

## Membuat Layout Sederhana

Selanjutnya adalah membuat layout sederhana. Buat folder baru yang didalamnya sudah diisi file HTML dan CSS.      
Kemudian isi dengan code seperti ini :            


```bash
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div id="container">
            <header>
                <h1>Layout Sederhana</h1>
            </header>
            <nav>
                <a href="home.html" class="active">Home</a>
                <a href="artikel.html">Artikel</a>
                <a href="about.html">About</a>
                <a href="kontak.html">Kontak</a>
            </nav>
            <section id="hero"></section>
            <section id="wrapper">
                <section id="main"></section>
                <aside id="sidebar"></aside>
            </section>
            <footer>
                <p>&copy; 2021 - Universitas Pelita Bangsa</p>
            </footer>
        </div>
    </body>
</html>
```        

![Gambar 3](Screenshoots/Capture3.PNG)        