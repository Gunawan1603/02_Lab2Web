# 02_Lab2Web
TUGAS PERTEMUAN 3

PEMROGRAMAN WEB

TEKNIK INFORMATIKA

UNIVERSITAS PELITA BANGSA

NAMA  : GUNAWAN

NIM   : 312010191

KELAS : TI.20.B1

DOSEN : Agung Nugroho,S.Kom.,M.Kom

**Praktikum 2: CSS Dasar**

**Instruksi Praktikum**
1. Persiapkan text editor misalnya VSCode.
2. Buat file baru dengan nama lab2_css_dasar.html
3. Buat struktur dasar dari dokumen HTML.
4. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
5. Lakukan validasi dokumen css dengan mengakses https://jigsaw.w3.org/css-validator/5. 

**Langkah-langkah Praktikum**<br>
**1. Membuat dokumen HTML**<br>
Buatlah dokumen HTML seperti berikut:<br>

![02_Lab2Web](Gambar/01.Dokumen_HTML.jpg)

Selanjutnya buka pada brwoser untuk melihat hasilnya.

![02_Lab2Web](Gambar/02.Tampilan_Dokumen_HTML.jpg)

Gambar 01.Tampilan Dokumen HTML

**2. Mendeklarasikan CSS Internal**

Kemudian tambahkan deklarasi CSS internal seperti berikut pada bagian head dokumen.

![02_Lab2Web](Gambar/03.Deklarasi_CSS_internal.jpg)

Selanjutnya simpan perubahan yang ada, dan lakukan refresh pada browser untuk melihat
hasilnya.

![02_Lab2Web](Gambar/04.Penambahan_CSS_pada_HTML.jpg)

Gambar 02. Penambahan CSS pada HTML

**3. Menambahkan Inline CSS**

Kemudian tambahkan deklarasi inline CSS pada tag ``<p>`` seperti berikut.

   ``<p style="text-align: center; color: #ccd8e4;">``
   
![02_Lab2Web](Gambar/05.Menambahkan_Inline_CSS.jpg) 

Simpan kembali dan refresh kembali browser untuk melihat perubahannya.

![02_Lab2Web](Gambar/06.Penambahan_Inline_CSS.jpg)

Gambar 03. Penambahan Inline CSS

**4. Membuat CSS Eksternal**

Buatlah file baru dengan nama **style_eksternal.css** kemudian buatlah deklarasi CSS seperti berikut.

![02_Lab2Web](Gambar/07.Membuat_CSS_Eksternal.jpg)

Kemudian tambahkan tag ``<link>`` untuk merujuk file css yang sudah dibuat pada bagian ``<head>``

>``<head>``<br>
>``<!-- menyisipkan css eksternal -->``<br>
>``<link rel="stylesheet" ``
>``href="style_eksternal.css" type="text/css">``<br>
>``</head>``

![02_Lab2Web](Gambar/08.Menambahkan_tag_link_untuk_merujuk_file_css.jpg)

Selanjutnya refresh kembali browser untuk melihat perubahannya.

![02_Lab2Web](Gambar/09.Tampilan_Eksternal_CSS.jpg)

Gambar 04. Tampilan Eksternal CSS

**5. Menambahkan CSS Selector**

Selanjutnya menambahkan CSS Selector menggunakan ID dan Class Selector. Pada file
**style_eksternal.css**, tambahkan kode berikut.

![02_Lab2Web](Gambar/10.Menambahkan_CSS_Selector.jpg)

Kemudian simpan kembali dan refresh browser untuk melihat perubahannya.

![02_Lab2Web](Gambar/11.CSS_ID_dan_Class_Selector.jpg)

Gambar 05. CSS ID dan Class Selector

# Pertanyaan dan Tugas

1. Lakukan eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS
dengan mengacu pada CSS Cheat Sheet yang diberikan pada file terpisah dari modul ini.
>**Jawab:**
> Eksperimen dengan mengubah dan menambah properti dan nilai pada kode CSS :
>![02_Lab2Web](Gambar/15.eksperimenCSS.jpg)<br>
>Berikut tampilan pada Browser setelah di ubah nilai padaCSS :
>![02_Lab2Web](Gambar/16.Tampilan_browser_eksperimenCSS.jpg)<br>
2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}? berikan
penjelasannya!
>**Jawab:**
>Perbedaaannya jika hanya h1{} maka akan merubah semua yang ada didalam elemen h1, sedangkan #intro h1{} hanya akan merubah yang memiliki tag intro.
3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada
elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

>**Jawab:**
>jika ketiga CSS merubah elemen yang sama maka deklarasi tersebut akan mengikuti aturan prioritas dimana prioritas CSS nya seperti ini:
>1. inline CSS
>2. ID selector CSS
>3. internal CSS
>4. external CSS<br>
>contoh:
>ini adalah tampilan coding pada html testing dimana terdapat 2 kalimat yang memiliki elemen yang sama yaitu h1:<br>
>**Disini bisa dilihat sudah terdapat 2 css mencoba merubah warna text h1 :**
>![02_Lab2Web](Gambar/12.Test_deklarasian_CSS.jpg)<br>
>Sedangkan eksternal css berupa :
>![02_Lab2Web](Gambar/14.Test_deklarasian_CSS.jpg)<br>
>Dan hasil Tampilan Pada Browser adalah :
>![02_Lab2Web](Gambar/13.Test_deklarasian_CSS.jpg)<br>
>**jadi kesimpulan yaitu semakin spesifik CSS tersebut maka prioritas semakin tinggi**

4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut
terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser?
Berikan penjelasan dan contohnya! ``( <p id="paragraf-1" class="text-paragraf"> )``
>**Jawab:**
>Hasilnya sesuai dengan kesimpulan saya sebelumnya semakin spesifik css tersebut maka akan semakin tinggi prioritas css tersebut :
>![02_Lab2Web](Gambar/17.Tampilan_id_class.jpg)<br>

Disitu bisa dilihat terdapat 2 css yang merujuk ke elemen yang sama tapi 1 merujuk dengan id yang birisi **font 50px dan warna blueviolet** sedangkan yang satu lagi merujuk dengan class yang berisi **font 10px dan warna magenta**:<br>
>![02_Lab2Web](Gambar/18.Tampilan_id_class_css.jpg)<br>

>Berikut tampilan Pada Browser :
>![02_Lab2Web](Gambar/19.Tampilan_Browser_id_class_css.jpg)<br>
>Text **"3. GUNAWAN TUGAS 2 PEMROGRAMAN WEB"** tersebut mengikuti css **selector id** dari pada **selector class** dikarenakan **id lebih spesifik daripada class**.

Cukup sekian Penjelasan dari saya.

**Terimakasih**
 












