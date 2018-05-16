<html>
<body>
<h1>
<p align="center"><b>Software Testing Document</b></p>
</h1>
<p align="center"><b>Version 1.0.0 </b><br>
<p align="center">14 Mei 2018</b>
<p align="center">
<img src="http://i67.tinypic.com/2yuhmww.png"/>
</p>

<br><p align="center"><b> APLIKASI POS QR-CODE ANDROID</b><br>
<p align="center"><b>Aplikasi Menggunakan Kode QR
</b>
<p align="center">Kelompok 2 <br><br>
 Mochamad Faizal			(1603179)<br>
 Luqmanul Hakim				(1603076)<br>
 Inneke Widianti			(1603072)<br>
 Rizaluddin Sidqi Baihaqi	(1603082)<br><br><br>

<p align="center"><b>Jurusan Teknik Informatika</b><br>
<h3><p align="center"><b>Politeknik Negeri Indramayu</b><br><br></h3>
</p>
</body>
</html>

##

### BAB 1 Pendahuluan
__1.1 Tujuan Pembuatan Dokumen__ <br>
Dokumen ini digunakan sebagai panduan untuk melakukan pengujian terhadap perangkat lunak Aplikasi POS QR-Code. Dokumen ini dipakai untuk melihat kemampuan dari program yang telah dirancang agar sesuai dengan keinginan dari pengguna. Pembuatan dokumen ini ditujukan untuk menguji perangkat lunak Aplikasi POS QR-Code yang merupakan bagian dari tugas mata kuliah Rekayasa Perangkat Lunak.

__1.2 Deskripsi Umum Sistem__ <br>
Pada umumnya toko-toko yang tidak terlalu besar metode transaksi pembayarannya manual seperti ditulis dikertas lalu di jumlah dengan kalkulator, dengan metode seperti itu memakan waktu dan tidak efisien, karena untuk transaksi pembayaran harus cepat dan tepat patal jadinya jika penghitungan salah, toko dapat merugi, ditambah pohon-pohon yang ada di muka semakin menipis, ini terjadi karena pohon menjadi bahan baku pembuatan kertas, semakin sedikitnya pohon, bumi semakin panas dan cuaca pun tidak menentu, dan sudah jelas kerusakan alam sudah mulai terlihat akibat pohon-pohon dimuka bumi ini berkurang.

Oleh karena itu kelompok kami mempunyai ide yang mungkin dapat meminimalisir penggunaan kertas secara berlebihan, yaitu dengan membuat aplikasi point of sales dengan QR-Code berbasis android. Aplikasi menggunakan sistem scan kode QR untuk setiap jenisa makanan yang dijual pada toko-toko, dari sistemnya sendirinya digunakan oleh 4 user, yaitu pembeli, kasir/karyawan, pemilik toko dan admin.

Dari sistem pembeli menggunakan imei dan nomor telpon untuk mendaftar kan smartphonenya, jiak imei nya sudah didaftar kan dan di data diri diisi dengan data pembeli maka aplikasi tersebut sudah bisa digunakan. Pada sistem pembeli terdapat beberapa fungsi utama yaitu :
<ul><li> Pembeli dapat melihat harga makanan dengan melakukan sca QR Code.</li>
<li> Pembeli dapat melakukan Top Up agar pada saat transaksi pembayaran tidak mengeluarkan uang cash.</li>
<li> Pembeli dapat melihat jumlah harga dari makanan yang dibeli.</li>
<li> Rincian pembeli langsung diterima oleh kasir setelah pembeli selesai melakukan memilih makanan yang akan mereka beli.</li>
</ul>

Pada sitem karyawan memiliki fungsi utama yaitu :
<ul>
<li> Menerima rincian pembelian.</li>
<li> Mengisi dompet elektronik pembeli(Top Up).</li>
<li> Mamasukan data barang.</li>
<li> Transaksi pembayaran.</li>
</ul>

Pada sistem pemilik toko memiliki fungsi utama yaitu :
<ul>
<li> Melihat rekap data bulanan.</li>
<li> Melihat omset bulanan. </li>
<li> Melihat data barang. </li>
</ul>

Admin disini adalah super user yang mengelola setiap data sistem ini. Sistem admin memiliki beberpa fungi utama yaitu :
<ul>
<li> Menerima data pada tiap-tiap toko.</li>
<li> Aprovement jika ada pembel yang mendaftar.</li>
<li> Presentase jumlah produk yang banyak terjual pada tiap-tiap toko perbulan secara otomatis.</li>
</ul>

____1.2.1 Perpektif Umum Sistem yang diuji____ <br>
____1.2.2 Spesifikasi Fungsional dan Non Fungsional____ <br>
____1.2.3 Arsitektur____ <br>
____1.2.4 Struktur Chart Modul____ <br>

__1.3 Deskripsi Dokumen (Ikhtisar)__ <br>
Dalam dokumen ini berisi 3 bagian utama yaitu Pendahuluan, Identifikasi dan Rencana Pengujian, Deskripsi dan Uji Hasil.

__1.4 Definisi dan Singkatan__ <br>
Definisi, Akronim dan Singkatan  | Penjelasan
----------------- | -------------
STD/DUPL | Software Test Description/Dokumen Uji Perangkat Lunak
STD/DUPL | DUPL adalah dokumen yang menyatakan hasil perencanaan pengujian, deskripsi kasus uji yang diberlakukan serta hasil pengujian yang telah dilakukan.

__1.5 Dokumen Referensi__ <br>
Dokumen Referensi yang digunakan dalam pembuatan DUPL adalah :<br>
- Ernita H. GL03. Dokumen Uji Perangkat Lunak (DUPL) SDS. Bogor.


### BAB 2 Lingkungan Pengujian Perangkat Lunak
__2.1 Perangkat Lunak Pengujian__ <br>
Perangkat lunak ini (Aplikasi POS QR-Code) diujikan dengan beberapa perangkat lunak lain, yaitu:<br>
- Sistem operasi: Android, Windows
- Bahasa pemrograman: Java, HTML, PHP
- Database: MySQL

__2.2 Perangkat Keras Pengujian__ <br>
Perangkat keras yang diperlukan untuk menguji Aplikasi POS QR-Code ini adalah satu set smartphone dan laptop dengan spesifikasi:(cont table)

__2.3 Material Pengujian__ <br>
Pada program “Aplikasi POS QR-Code” ini seorang member dapat melakukan pendaftaran dan login melalui android.(cont)

__2.4 Sumber Daya Manusia__ <br>
Persyaratan sumber daya manusia yang akan terlibat dalam proses pengujian perangkat lunak ini adalah :<br>
- Memahami konsep pemrograman berorientasi objek dalam bahasa Java, HTML dan PHP.
- Memahami proses pengujian perangkat lunak berorientasi objek.
- Memahami konsep pemrograman database MySQL.

__2.5 Prosedur Umum Pengujian__ <br>
____2.5.1 Pengenalan dan Latihan____ <br>
Penguji aplikasi ini hanya diberikan latihan kembali tentang SQL, dan pengenalan lebih lanjut tentang Android Studio dan Java. Pada dasarnya penguji telah memiliki pengetahuan tentang hal yang disebutkan sebelumnya tetapi latihan yang diberikan hanya bersifat penyegaran kembali.

____2.5.2 Persiapan Awal____ <br>
______2.5.2.1 Persiapan Prosedural______ <br>
Pengujian ini dilakukan di dalam lingkungan kampus. Dimana pengujian ini dilakukan oleh tim penguji yang telah di tentukan oleh Dosen mata kuliah Rekayasa Perangkat Lunak (RPL). Alat yang digunakan 1 buah smartphone dan 1 buah laptop dengan software yang telah di instalasi.

______2.5.2.2 Persiapan Perangkat Keras______ <br>
Perangkat keras yang perlu dipesiapkan adalah :<br>
Sebuah perangkat komputer yang dilengkapi dengan :(cont table)

______2.5.2.3 Persiapan Perangkat Lunak______ <br>
Persiapan yang harus dilakukan untuk menyiapkan perangkat lunak untuk diuji di lingkungan sistem operasi Android adalah sebagai berikut : (cont)<br>

Persiapan yang harus dilakukan untuk menyiapkan perangkat lunak untuk diuji di lingkungan sistem operasi Android adalah sebagai berikut : (cont)

____2.5.3 Pelaksanaan____ <br>
Pelaksanaan pengujian dilakukan dengan mengeksekusi perangkat lunak Aplikasi POS QR-Code dengan mengikuti skenario tertentu yang dibuat berdasarkan skenario yang terdapat pada dokumen SKPL-Aplikasi POS QR-Code.

____2.5.4 Pelaporan Hasil____ <br>
Dokumen hasil uji dari aplikasi ini akan diberikan kepada dosen Rekayasa Perangkat Lunak dan dievaluasi oleh dosen Rekayasa Perangkat Lunak dan kelompok lain yang bertindak sebagai klien dari kelompok kami. Sehingga aplikasi mendapatkan umpan balik dalam pengembangan perangkat lunak ini selanjutnya.

### BAB 3 Identifikasi dan Rencana Pengujian
__3.1 Object yang diuji__ <br>

__3.2 Kasus Uji__ <br>

__3.3 Teknik Pengujian yang dipakai__ <br>

__3.4 Expected result__ <br>

### BAB 4 Deskripsi dan Hasil Uji


### BAB 5 Analisis Hasil
