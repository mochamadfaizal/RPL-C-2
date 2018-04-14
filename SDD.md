<html>
<body>
<h1>
<p align="center"><b>Software Design Description</b></p>
</h1>
<p align="center"><b>Version 1.0.4 </b><br>
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
- IEEE. 1998. IEEE Recommended Practice for Software Requirement Specification. New York : IEEE.
- Pressman, Roger S. 2001. Software engineering: a practitioner’s approach 5th ed. New York : McGraw-Hill Companies, Inc.
- Dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) Super Monster Mall.

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

Deskripsi tabel-tabel yang terdapat pada database pembuatan aplikasi POS Menggunakan QR-CODE Scanner ini adalah sebagai berikut :

**Tabel User**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_user| Integer| 11 | Primary Key| Iya |Auto_increment| id user auto increment |
| email| varchar| 20 | Tidak | Tidak | -| email yang digunakan user untuk login |
| password| varchar| 20 | Tidak | Tidak | - |password yang digunakan user untuk login |
| level| varchar| 20 | Tidak | Tidak | -|level user untuk login seperti member, karyawan, admin, dan pemilik toko |

**Tabel Member**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_member| Integer| 11 | Primary Key| Iya |Auto_increment| id member auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| relasi untuk menghubungkan akun user dengan data member |
| nama| varchar| 20 | Tidak | Tidak | - |nama member  |
| email| varchar| 20 | Tidak | Tidak | -|email member |
| alamat| varchar| 80 | Tidak | Tidak | -|alamat member |
| no_hp| varchar| 15 | Tidak | Tidak | -|nomor hp member |
| jumlah_saldo| integer| 11 | Tidak | Tidak | -|jumlah saldo member |

**Tabel Toko**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_toko| Integer| 11 | Primary Key| Iya |Auto_increment| id toko auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| relasi untuk menghubungkan akun user dengan data toko |
| nama_toko| varchar| 20 | Tidak | Tidak | - |nama toko  |
| nama_pemilik_toko| varchar| 20 | Tidak | Tidak | -|nama pemilik toko |
| alamat_toko| varchar| 80 | Tidak | Tidak | -|alamat toko |
| email| varchar| 20 | Tidak | Tidak | -|email pemilik toko atau email toko |
| jumlah_saldo| integer| 11 | Tidak | Tidak | -|jumlah saldo toko |

**Tabel Karyawan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_karyawan| Integer| 11 | Primary Key| Iya |Auto_increment| id karyawan auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| relasi untuk menghubungkan akun user dengan data karyawan |
| id_toko| varchar| 20 | Tidak | Foreign Key | id_toko pada tabel toko |relasi untuk menghubungkan data karyawan dengan data toko  |
| nama| varchar| 20 | Tidak | Tidak | -|nama karyawan |
| email| varchar| 20 | Tidak | Tidak | -|email karyawan |
| no_hp| varchar| 15 | Tidak | Tidak | -|nomor hp karyawan |
| alamat| varchar| 80 | Tidak | Tidak | -|alamat karyawan |

**Tabel Pemasok**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_pemasok| Integer| 11 | Primary Key| Iya |Auto_increment| id pemasok auto increment |
| id_toko| varchar| 20 | Tidak | Foreign Key | id_toko pada tabel toko |relasi untuk menghubungkan data pemasok dengan data toko |
| nama| varchar| 20 | Tidak | Tidak | -|nama pemasok |
| no_hp| varchar| 15 | Tidak | Tidak | -|nomor hp pemasok |
| alamat| varchar| 80 | Tidak | Tidak | -|alamat pemasok |

**Tabel Barang**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_barang| Integer| 11 | Primary Key| Iya |Auto_increment| id barang auto increment |
| id_toko| varchar| 20 | Tidak | Foreign Key | id_toko pada tabel toko |relasi untuk menghubungkan data barang dengan data toko |
| nama_barang| varchar| 20 | Tidak | Tidak | -|nama barang |
| harga_beli| integer| 11 | Tidak | Tidak | -|harga beli barang |
| harga_jual| integer| 11 | Tidak | Tidak | -|harga jual barang|
| satuan| varchar| 10 | Tidak | Tidak | -|satuan dari barang |
| stok| integer| 11 | Tidak | Tidak | -|stok barang yang tersedia di toko |

**Tabel Transaksi_Penjualan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_jual| Integer| 11 | Primary Key| Iya |Auto_increment| id transaksi penjualan auto increment |
| id_toko| integer| 11 | Tidak | Foreign Key | id_toko pada tabel toko |relasi untuk menghubungkan data transaksi penjualan dengan data toko |
| id_member| integer| 11 | Tidak | Foreign Key | id_member pada tabel member |relasi untuk menghubungkan data transaksi penjualan dengan data member |
| id_karyawan| integer| 11 | Tidak | Foreign Key | id_karyawan pada tabel karyawan |relasi untuk menghubungkan data transaksi penjualan dengan data karyawan |
| tanggal| date| - | Tidak | Tidak | - |tanggal transaksi penjualan dilakukan |
| total_harga| int| 11 | Tidak | Tidak | -|total harga dari transaksi penjualan |
| cara_pembayaran| varchar| 20 | Tidak | Tidak | -|cara pembayaran member saat transaksi penjualan |


**Tabel Detail_Transaksi_Penjualan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_detail_jual| Integer| 11 | Primary Key| Iya |Auto_increment| id detail transaksi penjualan auto increment |
| id_jual| integer| 11 | Tidak | Foreign Key | id_jual pada tabel transaksi_penjualan |relasi untuk menghubungkan data detail transaksi penjualan dengan data transaksi penjualan |
| id_barang| integer| 11 | Tidak | Foreign Key | id_barang pada tabel barang |relasi untuk menghubungkan data detail transaksi penjualan dengan data barang |
| quantity| integer| 11 | Tidak | Tidak | - |quantity dari barang yang di jual |
| harga| integer| 11 | Tidak | Tidak | - |harga barang setelah dikali dengan quantity |

**Tabel Transaksi_Pembelian**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_beli| Integer| 11 | Primary Key| Iya |Auto_increment| id transaksi pembelian auto increment |
| id_toko| integer| 11 | Tidak | Foreign Key | id_toko pada tabel toko |relasi untuk menghubungkan data transaksi pembelian dengan data toko |
| id_pemasok| integer| 11 | Tidak | Foreign Key | id_pemasok pada tabel pemasok |relasi untuk menghubungkan data transaksi pembelian dengan data pemasok |
| id_karyawan| integer| 11 | Tidak | Foreign Key | id_karyawan pada tabel karyawan |relasi untuk menghubungkan data transaksi pembelian dengan data karyawan |
| tanggal| date| - | Tidak | Tidak | - |tanggal transaksi pembelian dilakukan |
| total_harga| int| 11 | Tidak | Tidak | -|total harga dari transaksi pembelian |


**Tabel Detail_Transaksi_Pembelian**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_detail_beli| Integer| 11 | Primary Key| Iya |Auto_increment| id detail transaksi pembelian auto increment |
| id_beli| integer| 11 | Tidak | Foreign Key | id_beli pada tabel transaksi_pembelian |relasi untuk menghubungkan data detail transaksi pembelian dengan data transaksi pembelian |
| id_barang| integer| 11 | Tidak | Foreign Key | id_barang pada tabel barang |relasi untuk menghubungkan data detail transaksi pembelian dengan data barang |
| quantity| integer| 11 | Tidak | Tidak | - |quantity dari barang yang di beli |
| harga| integer| 11 | Tidak | Tidak | - |harga barang setelah dikali dengan quantity |



____2.2.1 Definisi Domain/Type____ <br>

**Data User**

| Domain Name | Power Designer Type |
|---------|---------|
|id_user|primary key|
|email|string|
|password|string|
|level|string|

**Data Toko**

| Domain Name | Power Designer Type |
|---------|---------|
| id_toko|primary key|
| id_user|foreign key|
| nama_toko|string|
| nama_pemilik_toko|string|
| alamat_toko|string|
| email| string|
| jumlah_saldo|number|

**Data Member**

| Domain Name | Power Designer Type |
|---------|---------|
| id_member|primary key|
| id_user|foreign key|
| nama|string|
| email|string|
| alamat|string|
| no_hp|string|
| jumlah_saldo|number|


**Data Karyawan**

| Domain Name | Power Designer Type |
|---------|---------|
| id_karyawan|primary key|
| id_user|foreign key|
| id_toko|foreign key|
| nama|string|
| email|string|
| no_hp|string|
| alamat|string|


**Data Pemasok**

| Domain Name | Power Designer Type |
|---------|---------|
| id_pemasok|primary key|
| id_toko|foreign key|
| nama|string|
| no_hp|string|
| alamat|string|


**Data Barang**

| Domain Name | Power Designer Type |
|---------|---------|
| id_barang|primary key|
| id_toko|foreign key|
| nama_barang|string|
| harga_beli|number|
| harga_jual|number|
| satuan|string|
| stok|number|


**Data Transaksi Penjualan**

| Domain Name | Power Designer Type |
|---------|---------|
| id_jual|primary key|
| id_toko|foreign key|
| id_member|foreign key|
| id_karyawan|foreign key|
| tanggal|date|
| total_harga|number|
| cara_pembayaran|string|


**Data Detail Transaksi Penjualan**

| Domain Name | Power Designer Type |
|---------|---------|
| id_detail_jual|primary key|
| id_jual|foreign key|
| id_barang|foreign key|
| quantity|number|
| harga|number|

**Data Transaksi Pembelian**

| Domain Name | Power Designer Type |
|---------|---------|
| id_beli|primary key|
| id_toko|foreign key|
| id_member|foreign key|
| id_karyawan|foreign key|
| tanggal|date|
| total_harga|number|


**Data Detail Transaksi Pembelian**

| Domain Name | Power Designer Type |
|---------|---------|
| id_detail_beli|primary key|
| id_beli|foreign key|
| id_barang|foreign key|
| quantity|number|
| harga|number|



____2.2.2 Conceptual Data Model____ <br>

____2.2.3 Physical Data Model____ <br>

____2.2.4 Daftar Tabel Aplikasi____ <br>
| Nama Tabel | Primary Key | Data Store | E/R | Deskripsi Isi |
| --------- | --------- | --------- | --------- | --------- |
| - | - | - | - | - |

__2.3 Deskripsi Modul__ <br>
| No | Nama Modul | Keterangan |
| --------- | --------- | --------- |
| - | - | - |

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
Identifikasi/Nama : 
Deskripsi Isi : 
Jenis : 
Volume : 
Laju : 
Primary Key : 

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| - | - | - | - | - | - |

____3.2.2 Tabel____ <br>
Identifikasi/Nama : 
Deskripsi Isi : 
Jenis : 
Volume : 
Laju : 
Primary Key : 

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| - | - | - | - | - | - |

__3.3 Deskripsi Rinci Modul__ <br>

____3.3.1 Modul____ <br>

______3.3.1.1 Fungsi Modul______ <br>
| No | Fungsi | Jenis | Tabel Terkait |
| --------- | --------- | --------- | --------- |
| - | - | - | - |

______3.3.1.2 Spesifikasi Layar Utama______ <br>

______3.3.1.3 Spesifikasi Query______ <br>

______3.3.1.4 Spesifikasi Field Data Layar______ <br>

______3.3.1.5 Spesifikasi Objek-objek pada Layar______ <br>

______3.3.1.6 Spesifikasi Proses/Algoritma______ <br>

__3.4 Matriks Kerunutan__ <br>
