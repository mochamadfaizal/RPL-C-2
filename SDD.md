<html>
<body>
<h1>
<p align="center"><b>Software Design Description</b></p>
</h1>
<p align="center"><b>Version 1.0.0 </b><br>
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
__1.1 Tujuan__ <br>
Tujuan pembuatan SDD (Software Design Description) ini adalah untuk menjelaskan
langkah langkah desain dan proses-proses dalam pembuatan sistem aplikasi yang akan
diterapkan pada Aplikasi Pos QR-Code berbasis Android, dan juga memberi definisi kebutuhan
untuk sistem, spesifikasi kebutuhan fungsional.<br>

Dokumen perancangan ini dibuat berdasarkan spesifikasi kebutuhan Aplikasi Pos QR-Code berbasis Android yang akan dibuat. Dalam rangka membangun aplikasi tersebut, tentunya deskripsi perancangan untuk aplikasi tersebut dibutuhkan, khususnya oleh para pengembang dan pembangun aplikasi tersebut.<br>

Fungsi utama dari Aplikasi ini adalah membantu member untuk pengecekan harga produk yang dijual dengan cara scan Qr-code yang ada pada tiap-tiap jenis produk, dan juga dapat membantu saran transaksi agar tidak antri terlalu saat di kasir.<br>

__1.2 Lingkup__ <br>
Aplikasi Pos QR-Code adalah sebuah aplikasi berbasis android yang mempermudah dalam sarana transaksi dan pengecekan harga bagi member. Sistem di Aplikasi Pos QR-Code disebut dengan Q_Pa System. Pengguna aplikasi ini dapat melakukan pendaftaran, sign in, melihat harga dengan cara scan, memilih produk, mengisi jumlah produk yang diinginkan, dan melakukan pembayaran. Sistem ini dikelola oleh seorang admin yang bertugas memperbaharui katalog, data pelanggan, dan data tiap-tiap toko. Data-data yang dikelola admin dipertanggungjawabkan kepada Monster’s Corporation di mana seorang manajer dari Monster’s Corporation akan mengunjungi Super Monster Mall dan melakukan observasi serta meminta laporan pertanggungjawaban.<br>

__1.3 Definisi, Akronim dan Singkatan__ <br>

Definisi, Akronim dan Singkatan  | Penjelasan
----------------- | -------------
DFD  | Data Flow Diagram. Diagram yang menggambarkan aliran data
ERD  | Entity Relationship Diagram. Diagram yang menggambarkan entitas suatu objek beserta relasinya.
SKPL | Spesifikasi Kebutuhan Perangkat Lunak. Sebuah dokumen yang berisi analisis terhadap suatu perangkat lunak yang akan dibangun yang dijabarkan dalam suatu spesifikasi kebutuhan.
User | Pengguna Aplikasi
Admin | Pengelola Sistem  Aplikasi.

<br>


### BAB 2 Referensi <br>

Dokumen ini memiliki beberapa referensi dalam pembuatannya, yaitu sebagai berikut: <br>
<ul> <li>IEEE. 1998. IEEE Recommended Practice for Software Requirement Specification. New York : IEEE
<li>Pressman, Roger S. 2001. Software engineering: a practitioner’s approach 5th ed. New York : McGraw-Hill Companies, Inc.</li>
<li>Dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) Super Monster Mall</li></ul>

### BAB 3 Data Flow Diagram <br>

<ul>
<li>Context Diagram</li><br>
![Context](http://i66.tinypic.com/1z4d734.jpg)

<br>
<li>DFD Level 0</li><br>
![LV0](http://i67.tisnypic.com/169rark.jpg)

<br>
<li>DFD Level 1 Mengelola Data Toko</li><br>
![LV1TOKO](http://i64.tinypic.com/1xzdp4.jpg)

<br>
<li>DFD Level 1 Mengelola Data Karyawan</li><br>
![LV1KARYAWAN](http://i67.tinypic.com/2i8hcaf.jpg)

<br>
<li>DFD Level 1 Mengelola Data Barang</li><br>
![LV1BARANG](http://i64.tinypic.com/w2j67p.jpg)

<br>
<li>DFD Level 1 Mengelola Data Member</li><br>
![LV1MEMBER](http://i67.tinypic.com/uq4g2.jpg)