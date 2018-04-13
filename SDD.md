<html>
<body>
<h1>
<p align="center"><b>Software Design Description</b></p>
</h1>
<p align="center"><b>Version 1.0.3 </b><br>
<p align="center">5 Maret 2018</b>
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
Tujuan pembuatan SDD (Software Design Description) ini adalah untuk menjelaskan langkah langkah desain dan proses-proses dalam pembuatan sistem aplikasi yang akan diterapkan pada Aplikasi Pos QR-Code berbasis Android, dan juga memberi definisi kebutuhan untuk sistem, spesifikasi kebutuhan fungsional.<br>

Dokumen perancangan ini dibuat berdasarkan spesifikasi kebutuhan Aplikasi Pos QR-Code berbasis Android yang akan dibuat. Dalam rangka membangun aplikasi tersebut, tentunya deskripsi perancangan untuk aplikasi tersebut dibutuhkan, khususnya oleh para pengembang dan pembangun aplikasi tersebut.<br>

Fungsi utama dari Aplikasi ini adalah membantu member untuk pengecekan harga produk yang dijual dengan cara scan Qr-code yang ada pada tiap-tiap jenis produk, dan juga dapat membantu saran transaksi agar tidak antri terlalu saat di kasir.<br>

__1.2 Lingkup Masalah__ <br>
Aplikasi Pos QR-Code adalah sebuah aplikasi berbasis android yang mempermudah dalam sarana transaksi dan pengecekan harga bagi member. Sistem di Aplikasi Pos QR-Code disebut dengan Q_Pa System. Pengguna aplikasi ini dapat melakukan pendaftaran, sign in, melihat harga dengan cara scan, memilih produk, mengisi jumlah produk yang diinginkan, dan melakukan pembayaran. Sistem ini dikelola oleh seorang admin yang bertugas memperbaharui katalog, data pelanggan, dan data tiap-tiap toko. Data-data yang dikelola admin dipertanggungjawabkan kepada Monster’s Corporation di mana seorang manajer dari Monster’s Corporation akan mengunjungi Super Monster Mall dan melakukan observasi serta meminta laporan pertanggungjawaban.<br>

__1.3 Definisi, Akronim dan Singkatan__ <br>

Definisi, Akronim dan Singkatan  | Penjelasan
----------------- | -------------
DPPL/SDD | Deskripsi  Perancangan Perangkat Lunak	atau Software Design Description, merupakan deskripsi dari perangkat lunak yang akan dikembangkan.
SKPL/SRS | Spesifikasi Kebutuhan Perangkat Lunak atau Software Requirement Specification, merupakan dokumentasi kebutuhan perangkat lunak.
DFD | Data Flow Diagram, diagram dan notasi yang digunakan untuk menunjukkan aliran data pada perangkat lunak.
ERD |	Entity Relationship Diagram, diagram dan notasi yang digunakan untuk merepresentasikan struktur data statis pada perangkat lunak.
User | Pengguna Aplikasi
Admin | Pengelola Sistem  Aplikasi.

__1.4 Aturan Penamaan dan Penomoran__ <br>

__1.5 Referensi__ <br>
Dokumen ini memiliki beberapa referensi dalam pembuatannya, yaitu sebagai berikut: <br>
<ul> <li>IEEE. 1998. IEEE Recommended Practice for Software Requirement Specification. New York : IEEE
<li>Pressman, Roger S. 2001. Software engineering: a practitioner’s approach 5th ed. New York : McGraw-Hill Companies, Inc.</li>
<li>Dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) Super Monster Mall</li></ul>

__1.6 Ikhtisar Dokumen__<br>
Dokumen SDD ini dibagi menjadi tiga bagian utama. Bagian pertama berisi penjelasan tentang dokumen SDD yang mencakup tujuan pembuatan dokumen ini, lingkup masalah yang diselesaikan oleh perangkat lunak yang dikembangkan, definisi, referensi dan deskripsi umum. Bagian kedua berisi diagram dan spesifikasi kelas, komponen sistem dan arsitektur sistem dari Q-PAY yang telah dispesifikasikan pada dokumen SRS. Bagian ketiga berisi deskripsi rinci masing-masing kelas.

##

### BAB 2 Deksripsi Perancangan Global
__2.1 Rancangan Lingkungan Implementasi__ <br>
Aplikasi ini akan dikembangkan pada lingkungan dengan spesifikasi sebagai berikut :
-	Sistem Operasi	: Android, Windows
-	Bahasa Pemrograman	: Java, PHP, HTML
-	DBMS	: MySQL
-	Tools	: Android Studio, XAMPP, Sublime Text

__2.2 Deskripsi Data__ <br>
<ul><li>Nama table	: admin </li>
 <li>Volume	: </li>
 <li>Primary key	:id_admin</li>
 <li>Constraint integrity	: </li>
<li>Tabel admin adalah tabel basis data yang berisi data dari admin yang mengelola sistem.</li></ul>

____2.2.1 Definisi Domain/Type____ <br>

____2.2.2 Conceptual Data Model____ <br>

____2.2.3 Physical Data Model____ <br>

____2.2.4 Daftar Tabel Aplikasi____ <br>

__2.3 Deskripsi Modul__ <br>

### BAB 3 Deskripsi Perancangan Rinci <br>
__3.1 Diagram Konteks__ <br>
* Context Diagram
![Context](http://i68.tinypic.com/30sd175.jpg)

____3.1.1 DFD Level 0____ <br>
* DFD Level 0
![LV0]( http://i66.tinypic.com/2aak55j.jpg)

____3.1.2 DFD Level 1 Mengelola Data Master____ <br>
* DFD Level 1 Mengelola Data Master
![LV1TOKO](http://i67.tinypic.com/24qnv40.jpg)

____3.1.3 DFD Level 2 Mengelola Data Toko____ <br>
* DFD Level 2 Mengelola Data Toko
![LV1TOKO](http://i64.tinypic.com/jkc93c.jpg)

____3.1.4 DFD Level 2 Mengelola Data Karyawan____ <br>
* DFD Level 2 Mengelola Data Karyawan
![LV1KARYAWAN](http://i64.tinypic.com/2ni1jif.jpg)

____3.1.5 DFD Level 2 Mengelola Data Barang____ <br>
* DFD Level 2 Mengelola Data Barang
![LV1BARANG](http://i65.tinypic.com/f9fqki.jpg )

____3.1.6 DFD Level 1 Mengelola Data Member____ <br>
* DFD Level 1 Mengelola Data Member
![LV1MEMBER](http://i65.tinypic.com/k0jy9l.jpg)

__3.2 Deskripsi Rinci Tabel__ <br>

____3.2.1 Tabel____ <br>

__3.3 Deskripsi Rinci Modul__ <br>

____3.3.1 Modul____ <br>

______3.3.1.1 Fungsi Modul______ <br>

______3.3.1.2 Spesifikasi Layar Utama______ <br>

______3.3.1.3 Spesifikasi Query______ <br>

______3.3.1.4 Spesifikasi Field Data Layar______ <br>

______3.3.1.5 Spesifikasi Objek-objek pada Layar______ <br>

______3.3.1.6 Spesifikasi Proses/Algoritma______ <br>

__3.4 Matriks Kerunutan__ <br>
