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
| id_user| Integer| 11 | Primary Key| Iya |Auto_increment| Id user auto increment |
| email| Varchar| 20 | Tidak | Tidak | -| Email yang digunakan user untuk login |
| password| Varchar| 20 | Tidak | Tidak | - |Password yang digunakan user untuk login |
| level| Varchar| 20 | Tidak | Tidak | -|Level user untuk login seperti member, karyawan, admin, dan pemilik toko |

**Tabel Member**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_member| Integer| 11 | Primary Key| Iya |Auto_increment| Id member auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| Relasi untuk menghubungkan akun user dengan data member |
| nama| Varchar| 20 | Tidak | Tidak | - |Nama member  |
| email| Varchar| 20 | Tidak | Tidak | -|Email member |
| alamat| Varchar| 80 | Tidak | Tidak | -|Alamat member |
| no_hp| Varchar| 15 | Tidak | Tidak | -|Nomor hp member |
| jumlah_saldo| Integer| 11 | Tidak | Tidak | -|Jumlah saldo member |

**Tabel Toko**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_toko| Integer| 11 | Primary Key| Iya |Auto_increment| Id toko auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| Relasi untuk menghubungkan akun user dengan data toko |
| nama_toko| Varchar| 20 | Tidak | Tidak | - |Nama toko  |
| nama_pemilik_toko| Varchar| 20 | Tidak | Tidak | -|Nama pemilik toko |
| alamat_toko| Varchar| 80 | Tidak | Tidak | -|Alamat toko |
| email| Varchar| 20 | Tidak | Tidak | -|Email pemilik toko atau email toko |
| jumlah_saldo| Integer| 11 | Tidak | Tidak | -|Jumlah saldo toko |

**Tabel Karyawan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_karyawan| Integer| 11 | Primary Key| Iya |Auto_increment| Id karyawan auto increment |
| id_user| Integer| 11 | Tidak | Foreign Key | id user pada tabel user| Relasi untuk menghubungkan akun user dengan data karyawan |
| id_toko| Integer| 20 | Tidak | Foreign Key | id_toko pada tabel toko |Relasi untuk menghubungkan data karyawan dengan data toko  |
| nama| Varchar| 20 | Tidak | Tidak | -|Nama karyawan |
| email| Varchar| 20 | Tidak | Tidak | -|Email karyawan |
| no_hp| Varchar| 15 | Tidak | Tidak | -|Nomor hp karyawan |
| alamat| Varchar| 80 | Tidak | Tidak | -|Alamat karyawan |

**Tabel Pemasok**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_pemasok| Integer| 11 | Primary Key| Iya |Auto_increment| Id pemasok auto increment |
| id_toko| Integer| 20 | Tidak | Foreign Key | id_toko pada tabel toko |Relasi untuk menghubungkan data pemasok dengan data toko |
| nama| Varchar| 20 | Tidak | Tidak | -|Nama pemasok |
| no_hp| Varchar| 15 | Tidak | Tidak | -|Nomor hp pemasok |
| alamat| Varchar| 80 | Tidak | Tidak | -|Alamat pemasok |

**Tabel Barang**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_barang| Integer| 11 | Primary Key| Iya |Auto_increment| Id barang auto increment |
| id_toko| Integer| 20 | Tidak | Foreign Key | id_toko pada tabel toko |Relasi untuk menghubungkan data barang dengan data toko |
| nama_barang| Varchar| 20 | Tidak | Tidak | -|Nama barang |
| harga_beli| Integer| 11 | Tidak | Tidak | -|Harga beli barang |
| harga_jual| Integer| 11 | Tidak | Tidak | -|Harga jual barang|
| satuan| Varchar| 10 | Tidak | Tidak | -|Satuan dari barang |
| stok| Integer| 11 | Tidak | Tidak | -|Stok barang yang tersedia di toko |

**Tabel Transaksi_Penjualan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_jual| Integer| 11 | Primary Key| Iya |Auto_increment| Id transaksi penjualan auto increment |
| id_toko| Integer| 11 | Tidak | Foreign Key | id_toko pada tabel toko |Relasi untuk menghubungkan data transaksi penjualan dengan data toko |
| id_member| Integer| 11 | Tidak | Foreign Key | id_member pada tabel member |Relasi untuk menghubungkan data transaksi penjualan dengan data member |
| id_karyawan| Integer| 11 | Tidak | Foreign Key | id_karyawan pada tabel karyawan |Relasi untuk menghubungkan data transaksi penjualan dengan data karyawan |
| tanggal| Date| - | Tidak | Tidak | - |Tanggal transaksi penjualan dilakukan |
| total_harga| Integer| 11 | Tidak | Tidak | -|Total harga dari transaksi penjualan |
| cara_pembayaran| Varchar| 20 | Tidak | Tidak | -|Cara pembayaran member saat transaksi penjualan |


**Tabel Detail_Transaksi_Penjualan**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_detail_jual| Integer| 11 | Primary Key| Iya |Auto_increment| Id detail transaksi penjualan auto increment |
| id_jual| Integer| 11 | Tidak | Foreign Key | id_jual pada tabel transaksi_penjualan |Relasi untuk menghubungkan data detail transaksi penjualan dengan data transaksi penjualan |
| id_barang| Integer| 11 | Tidak | Foreign Key | id_barang pada tabel barang |Relasi untuk menghubungkan data detail transaksi penjualan dengan data barang |
| quantity| Integer| 11 | Tidak | Tidak | - |Quantity dari barang yang di jual |
| harga| Integer| 11 | Tidak | Tidak | - |Harga barang setelah dikali dengan quantity |

**Tabel Transaksi_Pembelian**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_beli| Integer| 11 | Primary Key| Iya |Auto_increment| Id transaksi pembelian auto increment |
| id_toko| Integer| 11 | Tidak | Foreign Key | id_toko pada tabel toko |Relasi untuk menghubungkan data transaksi pembelian dengan data toko |
| id_pemasok| Integer| 11 | Tidak | Foreign Key | id_pemasok pada tabel pemasok |Relasi untuk menghubungkan data transaksi pembelian dengan data pemasok |
| id_karyawan| Integer| 11 | Tidak | Foreign Key | id_karyawan pada tabel karyawan |Relasi untuk menghubungkan data transaksi pembelian dengan data karyawan |
| tanggal| Date| - | Tidak | Tidak | - |Tanggal transaksi pembelian dilakukan |
| total_harga| Integer| 11 | Tidak | Tidak | -|Total harga dari transaksi pembelian |


**Tabel Detail_Transaksi_Pembelian**

|Nama Field  | Jenis    |  Volume  | Laju| Primary Key| contraint integrity| Deskripsi|
|------------|----------|----------|-------------|-----------|-----------|---------------------|
| id_detail_beli| Integer| 11 | Primary Key| Iya |Auto_increment| Id detail transaksi pembelian auto increment |
| id_beli| Integer| 11 | Tidak | Foreign Key | id_beli pada tabel transaksi_pembelian |Relasi untuk menghubungkan data detail transaksi pembelian dengan data transaksi pembelian |
| id_barang| Integer| 11 | Tidak | Foreign Key | id_barang pada tabel barang |Relasi untuk menghubungkan data detail transaksi pembelian dengan data barang |
| quantity| Integer| 11 | Tidak | Tidak | - |Quantity dari barang yang di beli |
| harga| Integer| 11 | Tidak | Tidak | - |Harga barang setelah dikali dengan quantity |



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
| User | id_user | D10 | - | Berisi email dan password user dengan level yang berbeda digunakan untuk login |
| Barang | id_barang | D1 | - | Berisi data barang yang ada di toko seperti nama, harga jual dan harga beli, serta stok persediaan |
| Karyawan | id_karyawan | D3 | - | Berisi data karyawan yang bekerja di toko |
| Toko | id_toko | D2 | - | Berisi data toko dan pemilik toko seperti nama toko, nama pemilik toko, alamat, email dan sebagainya |
| Pemasok | id_pemasok | D4 | - | Berisi data pemasok barang pada toko, pemasok yang memang sudah sering men-supplay barang di toko tersebut |
| Member | id_member | D5 | - | Berisi data diri member yang digunakan sebagai profil member pada apliksi |
| Transaksi_penjualan | id_jual | D6 | - | Berisi data dari setiap transaksi penjualan yang dilakukan toko dengan member |
| Detail_penjualan | id_detail_jual | D7 | - | Berisi data rincian dari setiap transaksi penjualan |
| Transaksi_pembelian | id_beli | D8 | - | Berisi data dari setiap transaksi pembelian yang dilakukan toko dengan pemasok |
| Detail_pembelian | id_detail_beli | D9 | - | Berisi data rincian dari setiap transaksi pembelian |



### BAB 3 Deskripsi Perancangan Rinci <br>
__3.1 Diagram Konteks__ <br>
<p align="justify">Diagram konteks adalah diagram yang terdiri dari suatu proses dan menggambarkan ruang lingkup suatu sistem. Diagram konteks merupakan level tertinggi dari DFD yang menggambarkan seluruh input ke dalam sistem atau output dari sistem yang memberi gambaran tentang keseluruhan sistem. Sistem dibatasi oleh boundary (Digambarkan dengan garis putus - putus). Dalam diagram konteks hanya ada satu proses, tidak boleh ada store dalam diagram konteks. Berikut ini adalah gambar diagram konteks dari sistem Aplikasi Q-Pay.</p>

* Context Diagram
![Context](http://i63.tinypic.com/2yzarmg.jpg)

____3.1.1 DFD Level 0____ <br>
Data Flow Diagram merupakan cara untuk memodelkan proses dalam analisis dan perancangan perangkat lunak, dan merupakan penjelasan dari context diagram. Dalam aplikasi ini terdapat 3 proses utama yaitu mengelola data master, mengelola transaksi dan mengelola data member.

* DFD Level 0
![LV0](http://i63.tinypic.com/2ewcgox.jpg)

____3.1.2 DFD Level 1 Mengelola Data Master____ <br>
DFD level 1 merupakan rincian dari dari level 0, dan pada dfd level 1 mengelola data master terdapat 4 proses yaitu mengelola data toko, mengelola data karyawan, mengelola data pemasok dan mengelola data barang.

* DFD Level 1 Mengelola Data Master
![LV1MASTER](http://i65.tinypic.com/2czwv8x.jpg)

____3.1.3 DFD Level 2 Mengelola Data Toko____ <br>
DFD level 2 merupakan rincian dari dari level 1, dan pada dfd level 2 mengelola data toko terdapat 5 proses yaitu melakukan validasi, menambahkan data, mengubah data, menghapus data dan melihat data.

* DFD Level 2 Mengelola Data Toko
![LV2TOKO](http://i64.tinypic.com/2chrp5g.jpg)

____3.1.4 DFD Level 2 Mengelola Data Karyawan____ <br>
DFD level 2 merupakan rincian dari dari level 1, dan pada dfd level 2 mengelola data karyawan terdapat 5 proses yaitu melakukan validasi, menambahkan data, mengubah data, menghapus data dan melihat data.

* DFD Level 2 Mengelola Data Karyawan
![LV2KARYAWAN](http://i66.tinypic.com/5vdisg.jpg)

____3.1.5 DFD Level 2 Mengelola Data Barang____ <br>
DFD level 2 merupakan rincian dari dari level 1, dan pada dfd level 2 mengelola data barang terdapat 5 proses yaitu melakukan validasi, menambahkan data, mengubah data, menghapus data dan melihat data.

* DFD Level 2 Mengelola Data Barang
![LV2BARANG](http://i67.tinypic.com/25ti3gx.jpg)

____3.1.6 DFD Level 2 Mengelola Data Pemasok____ <br>
DFD level 2 merupakan rincian dari dari level 1, dan pada dfd level 2 mengelola data pemasok terdapat 5 proses yaitu melakukan validasi, menambahkan data, mengubah data, menghapus data dan melihat data.

* DFD Level 2 Mengelola Data Pemasok
![LV2PEMASOK](http://i63.tinypic.com/ivz9ug.jpg)

____3.1.7 DFD Level 1 Mengelola Data Member____ <br>
DFD level 1 merupakan rincian dari dari level 0, dan pada dfd level 1 mengelola data member terdapat 5 proses yaitu melakukan validasi, menambahkan data, mengubah data, menghapus data dan melihat data.

* DFD Level 1 Mengelola Data Member
![LV1MEMBER](http://i64.tinypic.com/2aj3qip.jpg)

____3.1.8 DFD Level 1 Mengelola Data Transaksi____ <br>
DFD level 1 merupakan rincian dari dari level 0, dan pada dfd level 1 mengelola data transaksi terdapat 3 proses yaitu melakukan konversi qr code dan hitung harga, transaksi penjualan, dan transaksi pembelian.

* DFD Level 1 Mengelola Data Transaksi
![LV1TRANSAKSI](http://i63.tinypic.com/2lvk0me.jpg)

__3.2 Deskripsi Rinci Tabel__ <br>

____3.2.1 Tabel User____ <br>
<br>Identifikasi/Nama : User
<br>Deskripsi Isi : Berisi semua user dalam aplikasi
<br>Jenis : Tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_user

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_user | merupakan key dari tabel user | int | No | - | Primary key yang unik setiap user, bersifat auto increment contoh : 1 |
| email | menyatakan email user | varchar(20) | No | - | Email akan digunakan sebagai username untuk login user |
| password | menyatakan password user | varchar(20) | No | - | password akan digunakan untuk login user, password harus sesuai dengan email agar login berhasil |
| level | menyatakan tingkatan user | varchar(20) | No | - | level digunakan untuk menyatakan tingkatan user, dimana terdapat 4 level yaitu admin, karyawab, pemilik toko, dan member |

____3.2.2 Tabel Member____ <br>
<br>Identifikasi/Nama : Member
<br>Deskripsi Isi : Berisi data profil member yang sudah melakukan registrasi
<br>Jenis : tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_member

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_member | merupakan key dalam tabel member | int | No | - | Primary key yang unik setiap member, bersifat auto increment contoh : 1 |
| id_user | merupakan foreign key yang terhubung dengan tabel user | int | No | - | Foreign key yang menghubungkan tabel member dengan user karena setiap member mempunyai data user yang digunakan untuk login |
| nama | menyatakan nama member | varchar(20) | No | - | Nama dari member |
| email | menyatakan email member | varchar(20) | No | - | Email dari member |
| alamat | menyatakan alamat member | varchar(50) | Yes | - | Alamat dari member |
| no_hp | menyatakan nomor hp member | varchar(15) | Yes | - | Nomor hp dari member |
| jumlah_saldo | menyatakan jumlah saldo member yang ada pada admin | int | No | 0 | Merupakan jumlah saldo dari member yang ada pada admin dan dapat digunakan pada saat transaksi dengan fitur top up atau e-cash |

____3.2.3 Tabel Toko____ <br>
<br>Identifikasi/Nama : Toko
<br>Deskripsi Isi : Berisi data toko yang sudah melakukan registrasi
<br>Jenis : tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_toko

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_toko | merupakan key dalam tabel toko | int | No | - | Primary key yang unik setiap toko, bersifat auto increment contoh : 1 |
| id_user | merupakan foreign key yang terhubung dengan tabel user | int | No | - | Foreign key yang menghubungkan tabel toko dengan user karena setiap toko mempunyai data user yang digunakan untuk login |
| nama_toko | menyatakan nama toko yang mendaftar | varchar(20) | No | - | Nama dari toko |
| nama_pemilik_toko | menyatakan nama pemilik toko | varchar(20) | No | - | Nama dari pemilik toko |
| alamat_toko | menyatakan alamat toko | varchar(50) | Yes | - | Alamat dari toko |
| email | menyatakan email toko | varchar(20) | No | - | Email dari toko atau pemilik toko |
| jumlah_saldo | menyatakan jumlah saldo toko yang ada pada admin | int | No | 0 | Merupakan jumlah saldo dari toko yang ada pada admin didapatkan dari transaksi dengan member yang menggunakan fitur top up atau e-cash |

____3.2.4 Tabel Karyawan____ <br>
<br>Identifikasi/Nama : Karyawan
<br>Deskripsi Isi : Berisi data karyawan yang sudah ditambahkan oleh pemilik toko
<br>Jenis : tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_karyawan

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_karyawan | merupakan key dalam tabel karyawan | int | No | - | Primary key yang unik setiap karyawan, bersifat auto increment contoh : 1 |
| id_user | merupakan foreign key yang terhubung dengan tabel user | int | No | - | Foreign key yang menghubungkan tabel karyawan dengan user karena setiap karyawan mempunyai data user yang digunakan untuk login |
| id_toko | merupakan foreign key yang terhubung dengan tabel toko | int | No | - | Foreign key yang menghubungkan tabel karyawan dengan toko karena setiap toko mempunyai data karyawan berbeda |
| nama | menyatakan nama karyawan | varchar(20) | No | - | Nama dari karyawan |
| email | menyatakan email karyawan | varchar(20) | No | - | Email dari karyawan |
| no_hp | menyatakan nomor hp karyawan | varchar(15) | Yes | - | Nomor hp dari karyawan |
| alamat | menyatakan alamat karyawan | varchar(50) | Yes | - | Alamat dari karyawan |


____3.2.5 Tabel Pemasok____ <br>
<br>Identifikasi/Nama : Pemasok
<br>Deskripsi Isi : Berisi data pemasok yang sudah ditambahkan oleh pemilik toko
<br>Jenis : tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_pemasok

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_pemasok | merupakan key dalam tabel pemasok | int | No | - | Primary key yang unik setiap pemasok, bersifat auto increment contoh : 1 |
| id_toko | merupakan foreign key yang terhubung dengan tabel toko | int | No | - | Foreign key yang menghubungkan tabel pemasok dengan toko karena setiap toko mempunyai data pemasok yang berbeda |
| nama | menyatakan nama pemasok | varchar(20) | No | - | Nama dari pemasok |
| no_hp | menyatakan nomor hp pemasok | varchar(15) | Yes | - | Nomor hp dari pemasok |
| alamat | menyatakan alamat pemasok | varchar(50) | Yes | - | Alamat dari pemasok |


____3.2.6 Tabel Barang____ <br>
<br>Identifikasi/Nama : Barang
<br>Deskripsi Isi : Berisi data barang yang sudah ditambahkan oleh karyawan ataupun pemilik toko
<br>Jenis : tabel referensi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_barang

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_barang | merupakan key dalam tabel barang | int | No | - | Primary key yang unik setiap barang, bersifat auto increment contoh : 1 |
| id_toko | merupakan foreign key yang terhubung dengan tabel toko | int | No | - | Foreign key yang menghubungkan tabel barang dengan toko karena setiap toko mempunyai data barang yang berbeda |
| nama_barang | menyatakan nama barang | varchar(20) | No | - | Nama dari barang |
| harga_jual | menyatakan harga jual dari barang | int | No | - | Harga barang yang akan dijual ke member |
| harga_beli | menyatakan harga beli dari barang | int | No | - | Harga barang yang dibeli dari pemasok |
| satuan | menyatakan satuan dari barang | int | No | - | Satuan dari barang, seperti kg, lusin, pak |
| stok | menyatakan stok dari barang | int | No | - | stok persediaan barang di toko |

____3.2.7 Tabel Transaksi Penjualan____ <br>
<br>Identifikasi/Nama : Transaksi penjualan
<br>Deskripsi Isi : Berisi data transaksi penjualan yang dilakukan toko dengan member
<br>Jenis : tabel transaksi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_jual

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_jual | merupakan key dalam tabel transaksi penjualan | int | No | - | Primary key yang unik setiap transaksi penjualan, bersifat auto increment contoh : 1 |
| id_toko | merupakan foreign key yang terhubung dengan tabel toko | int | No | - | Foreign key yang menghubungkan tabel transaksi penjualan dengan toko karena setiap toko mempunyai data tansaksi penjualan yang berbeda |
| id_member | merupakan foreign key yang terhubung dengan tabel member | int | No | - | Foreign key yang menghubungkan tabel transaksi penjualan dengan member karena setiap transaksi penjualan dilakukan dengan member yang berbeda |
| id_karyawan | merupakan foreign key yang terhubung dengan tabel karyawan | int | No | - | Foreign key yang menghubungkan tabel transaksi penjualan dengan karyawan karena setiap transaksi penjualan bisa saja dilakukan oleh karyawan yang berbeda |
| tanggal | menyatakan tanggal transaksi penjualan dilakukan | date | No | - | Berisi tanggal transaksi penjualan dilakukan |
| total_harga | menyatakan total harga yang harus dibayar oleh member | int | No | - | Jumlah harga barang yang harus dibayar member |
| cara_pembayaran | menyatakan cara pembayaran yang dilakukan oleh member | varchar(20) | No | - | Berisi hanya pilihan cash (bayar manual) ataupun top up (menggunakan saldo member yang ada pada admin |

____3.2.8 Tabel Detail Penjualan____ <br>
<br>Identifikasi/Nama : Detail Penjualan
<br>Deskripsi Isi : Berisi data rincian dari tabel transaksi penjualan
<br>Jenis : tabel transaksi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_detail_jual

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_detail_jual | merupakan key dalam tabel detail penjualan | int | No | - | Primary key yang unik setiap detail penjualan, bersifat auto increment contoh : 1 |
| id_jual | merupakan foreign key yang terhubung dengan tabel transaksi penjualan | int | No | - | Foreign key yang menghubungkan tabel detail penjualan dengan transaksi penjualan karena setiap transaksi penjualan mempunyai beberapa data detail penjualan  |
| id_barang | merupakan foreign key yang terhubung dengan tabel barang | int | No | - | Foreign key yang menghubungkan tabel detail penjualan dengan barang karena setiap detail penjualan mempunyai data barang yang lebih dari satu |
| quntity | menyatakan banyaknya barang detail penjualan | int | No | - | Jumlah atau quantity dari barang dari setiap transaksi penjualan |
| harga | menyatakan harga dari barang | int | No | - | Harga dari setiap barang dalam transaksi penjualan |


____3.2.9 Tabel Transaksi Pembelian____ <br>
<br>Identifikasi/Nama : Transaksi pembelian
<br>Deskripsi Isi : Berisi data transaksi pembelian barang yang dilakukan toko dengan pemasok
<br>Jenis : tabel transaksi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_beli

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_beli | merupakan key dalam tabel transaksi pembelian | int | No | - | Primary key yang unik setiap transaksi pembelian, bersifat auto increment contoh : 1 |
| id_toko | merupakan foreign key yang terhubung dengan tabel toko | int | No | - | Foreign key yang menghubungkan tabel transaksi pembelian dengan toko karena setiap toko mempunyai data tansaksi pembelian yang berbeda |
| id_pemasok | merupakan foreign key yang terhubung dengan tabel pemasok | int | No | - | Foreign key yang menghubungkan tabel transaksi pembelian dengan pemasok karena setiap transaksi pembelian dilakukan dengan pemasok yang berbeda |
| id_karyawan | merupakan foreign key yang terhubung dengan tabel karyawan | int | No | - | Foreign key yang menghubungkan tabel transaksi pembelian dengan karyawan karena setiap transaksi pembelian bisa saja dilakukan oleh karyawan yang berbeda |
| tanggal | menyatakan tanggal transaksi pembelian dilakukan | date | No | - | Berisi tanggal transaksi pembelian dilakukan |
| total_harga | menyatakan total harga yang harus dibayar oleh toko | int | No | - | Jumlah harga barang yang harus dibayar toko |

____3.2.10 Tabel Detail Pembelian____ <br>
<br>Identifikasi/Nama : Detail Pembelian
<br>Deskripsi Isi : Berisi data rincian dari tabel transaksi pembelian
<br>Jenis : tabel transaksi
<br>Volume : -
<br>Laju : -
<br>Primary Key : id_detail_beli

| Id Field | Deskripsi | Tipe & Length | Boleh NULL | Default | Keterangan |
| --------- | --------- | --------- | --------- | --------- | --------- |
| id_detail_beli | merupakan key dalam tabel detail pembelian | int | No | - | Primary key yang unik setiap detail pembelian, bersifat auto increment contoh : 1 |
| id_beli | merupakan foreign key yang terhubung dengan tabel transaksi pembelian | int | No | - | Foreign key yang menghubungkan tabel detail pembelian dengan transaksi pembelian karena setiap transaksi pembelian mempunyai beberapa data detail pembelian  |
| id_barang | merupakan foreign key yang terhubung dengan tabel barang | int | No | - | Foreign key yang menghubungkan tabel detail pembelian dengan barang karena setiap detail pembelian mempunyai data barang yang lebih dari satu |
| quntity | menyatakan banyaknya barang detail pembelian | int | No | - | Jumlah atau quantity dari barang dari setiap transaksi pembelian |
| harga | menyatakan harga dari barang | int | No | - | Harga dari setiap barang dalam transaksi pembelian |



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
