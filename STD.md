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
Perangkat lunak yang akan diuji adalah “Aplikasi POS QR-Code”. Perangkat lunak ini adalah perangkat lunak yang digunakan untuk
proses transaksi antara penjual dengan pembeli dan membantu pengelolaan data. Sistem ini diimplementasikan melalui komunikasi di media antara sesama pengguna dengan sistem.

____1.2.1 Perpektif Umum Sistem yang diuji____ <br>
____1.2.2 Spesifikasi Fungsional dan Non Fungsional____ <br>
____1.2.3 Arsitektur____ <br>
____1.2.4 Struktur Chart Modul____ <br>

__1.3 Deskripsi Dokumen (Ikhtisar)__ <br>
Dalam dokumen ini berisi 3 bagian utama yaitu Pendahuluan, Identifikasi dan Rencana Pengujian, Deskripsi dan Uji Hasil.

__1.4 Definisi dan Singkatan__ <br>
- SKPL adalah Spesifikasi Kebutuhan Perangkat Lunak, atau dalam bahasa Inggris-nya sering juga disebut sebagai Software Requirements Spesification (SRS), dan merupakan spesifikasi dari perangkat lunak yang akan dikembangkan
- DFD adalah Data Flow Diagram, diagram dan notasi yang digunakan untuk menunjukkan aliran data pada perangkat lunak.
- ERD adalah Entity Relationship Diagram, diagram dan notasi yang digunakan untuk merepresentasikan struktur data statis pada perangkat lunak.

__1.5 Dokumen Referensi__ <br>
Dokumen Referensi yang digunakan dalam pembuatan DUPL adalah :<br>
- Sistem Pencarian Pegawai.2013. Spesifikasi Kebutuhan Perangkat Lunak (SKPL) SPP. Bogor.
- Sistem Pencarian Pegawai. Dokumen Perancangan Perangkat Lunak (DPPL) SITBO. Bogor.
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
