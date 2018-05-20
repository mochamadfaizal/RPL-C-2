
<html>
<body>
<h1>
<p align="center"><b>Software Testing Document</b></p>
</h1>
<p align="center"><b>Version 1.1.0 </b><br>
<p align="center">14 Mei 2018</b>
<p align="center">
<img src="http://i67.tinypic.com/2yuhmww.png"/>
</p>

<br><p align="center"><b> APLIKASI POS QR-CODE ANDROID</b><br>
<p align="center"><b>Aplikasi Menggunakan Kode QR
</b>
<p align="center">Kelompok 2 <br><br>
 Mochamad Faizal			(1603079)<br>
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

__1.3 Deskripsi Dokumen (Ikhtisar)__ <br>
Dalam dokumen ini berisi 3 bagian utama yaitu Pendahuluan, Identifikasi dan Rencana Pengujian, Deskripsi dan Uji Hasil.

__1.4 Definisi dan Singkatan__ <br>

Definisi, Akronim dan Singkatan | Penjelasan |
--------------------------------| ---------- |
STD/DUPL | _Software Test Description_/Dokumen Uji Perangkat Lunak merupakan dokumen yang menyatakan hasil perencanaan pengujian, deskripsi kasus uji yang diberlakukan serta hasil pengujian yang telah dilakukan.|
SRS/SKPL | _Software Requirements Spesification_/Spesifikasi Kebutuhan Perangkat Lunak merupakan spesifikasi dari perangkat lunak yang akan dikembangkan.|
SDD/DPPL | _Software Design Description_/Deskripsi Perancangan Perangkat Lunak merupakan deskripsi dari perangkat lunak yang akan dikembangkan.|

__1.5 Dokumen Referensi__ <br>
Dokumen Referensi yang digunakan dalam pembuatan DUPL adalah :<br>
<ul>
<li>Ernita H. GL03. Dokumen Uji Perangkat Lunak (DUPL) SDS. Bogor.</li>
</ul>

### BAB 2 Lingkungan Pengujian Perangkat Lunak
__2.1 Perangkat Lunak Pengujian__ <br>
Perangkat lunak ini (Aplikasi POS QR-Code) diujikan dengan beberapa perangkat lunak lain, yaitu:<br>
<ul>
<li>Sistem operasi: Android, Windows</li>
<li>Bahasa pemrograman: Java, HTML, PHP</li>
<li>Database: MySQL</li>
</ul>

__2.2 Perangkat Keras Pengujian__ <br>
Perangkat keras yang diperlukan untuk menguji Aplikasi POS QR-Code ini adalah satu set smartphone dan laptop dengan spesifikasi:<br><br>
__Smartphone__
<ul>
<li>operating sistem : Andoid Nougat (7.0)</li>
<li>Bahasa Pemrograman : Java</li>
<li>Database : Mysql
</ul><br>

__Laptop__
<ul>
<li>Processor : Intel Pentium Dual Core</li>
<li>Memory : 4 GB DDR2</li?
<li>Harddisk : 500 GB</li>
</ul>

__2.3 Material Pengujian__ <br>
Pada program “Aplikasi POS QR-Code” ini seorang member dapat melakukan pendaftaran dan login melalui android, melakukan scan dan transaksi. Karyawan dapat mengelola barang dari android, dan melakukan transasksi. Pemilik toko dapat mengelola data karyawan, data barang, dan data pemasok melalui web. 

__2.4 Sumber Daya Manusia__ <br>
Persyaratan sumber daya manusia yang akan terlibat dalam proses pengujian perangkat lunak ini adalah :<br>
<ul>
<li>Memahami konsep pemrograman berorientasi objek dalam bahasa Java, HTML dan PHP.</li>
<li>Memahami proses pengujian perangkat lunak berorientasi objek.</li>
<li>Memahami konsep pemrograman database MySQL.</li>
</ul>

__2.5 Prosedur Umum Pengujian__ <br>
____2.5.1 Pengenalan dan Latihan____ <br>
Penguji aplikasi ini hanya diberikan latihan kembali tentang SQL, dan pengenalan lebih lanjut tentang Android Studio dan Java. Pada dasarnya penguji telah memiliki pengetahuan tentang hal yang disebutkan sebelumnya tetapi latihan yang diberikan hanya bersifat penyegaran kembali.

____2.5.2 Persiapan Awal____ <br>
______2.5.2.1 Persiapan Prosedural______ <br>
Pengujian ini dilakukan di dalam lingkungan kampus. Dimana pengujian ini dilakukan oleh tim penguji yang telah di tentukan oleh Dosen mata kuliah Rekayasa Perangkat Lunak (RPL). Alat yang digunakan 1 buah smartphone dan 1 buah laptop dengan software yang telah di instalasi.

______2.5.2.2 Persiapan Perangkat Keras______ <br>
Perangkat keras yang diperlukan untuk menguji Aplikasi POS QR-Code ini adalah satu set smartphone dan laptop dengan spesifikasi:<br>
__Smartphone__
<ul>
<li>operating sistem : Andoid Nougat (7.0)</li>
<li>Bahasa Pemrograman : Java</li>
<li>Database : Mysql
</ul>

__Laptop__
<ul>
<li>Processor : Intel Pentium Dual Core</li>
<li>Memory : 4 GB DDR2</li?
<li>Harddisk : 500 GB</li>
</ul>

______2.5.2.3 Persiapan Perangkat Lunak______ <br>
Persiapan yang harus dilakukan untuk menyiapkan perangkat lunak untuk diuji di lingkungan sistem operasi Android adalah sebagai berikut :<br>
__Smartphone__
<ul>
<li>operating sistem : Andoid Nougat (7.0)</li>
<li>Bahasa Pemrograman : Java</li>
<li>Database : Mysql
</ul>
Persiapan yang harus dilakukan untuk menyiapkan perangkat lunak untuk diuji di lingkungan sistem operasi Windows adalah sebagai berikut :<br>

__Laptop__
<ul>
<li>Processor : Intel Pentium Dual Core</li>
<li>Memory : 4 GB DDR2</li?
<li>Harddisk : 500 GB</li>
</ul>

____2.5.3 Pelaksanaan____ <br>
Pelaksanaan pengujian dilakukan dengan mengeksekusi perangkat lunak Aplikasi POS QR-Code dengan mengikuti skenario tertentu yang dibuat berdasarkan skenario yang terdapat pada dokumen SKPL-Aplikasi POS QR-Code.

____2.5.4 Pelaporan Hasil____ <br>
Dokumen hasil uji dari aplikasi ini akan diberikan kepada dosen Rekayasa Perangkat Lunak dan dievaluasi oleh dosen Rekayasa Perangkat Lunak dan kelompok lain yang bertindak sebagai klien dari kelompok kami. Sehingga aplikasi mendapatkan umpan balik dalam pengembangan perangkat lunak ini selanjutnya.

##
### BAB 3 Identifikasi dan Rencana Pengujian


<table>
	<thead>
		<tr>
			<td rowspan="2" align="center"><strong>Kelas Uji</strong></td>
			<td rowspan="2" align="center"><strong>Butir Uji</strong></td>
			<td colspan="2" align="center"><strong>Identifikasi</strong></td>
			<td rowspan="2" align="center"><strong>Jenis Pengujian</strong></td>
			<td rowspan="2" align="center"><strong>Teknik Pengujian</strong></td>
			<td rowspan="2" align="center"><strong>Penguji</strong></td>
		</tr>
		<tr>
			<td align="center"><strong>SRS-/SDD</strong></td>
			<td align="center"><strong>STD-</strong></td>
		</tr>
		<!-- <! Login User Mobile > -->
		<tr>
			<td rowspan="3" align="center"><strong>Login User Mobile</strong></td>
			<td>Username dan Password yang di masukkan sesuai data yang ada pada database</td>
			<td>SRS-2.2.1</td>
			<td>STD-1.0</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Username dan Password yang di masukkan tidak sesuai data yang ada pada database</td>
			<td>SRS-2.2.1</td>
			<td>STD-1.1</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td> 
		</tr>
		<tr>
			<td>Tidak mengisi form login </td>
			<td>SRS-2.2.1</td>
			<td>STD-1.2</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<!--  Register User Mobile  -->
		<tr>
			<td rowspan="3" align="center"><strong>Register Member</strong></td>
			<td>Mengisi form register sesuai dengan data yang diminta</td>
			<td>SRS-2.2.1</td>
			<td>STD-2.0</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td> 
		</tr>
		<tr>
			<td>Tidak mengisi form register</td>
			<td>SRS-2.2.1</td>
			<td>STD-2.1</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Mengisi email tidak sesuai dengan format yang diminta sistem (kurang karakter '@')</td>
			<td>SRS-2.2.1</td>
			<td>STD-2.2</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td> 
		</tr>
		 <!-- Data Barang Pada Karyawan --> 
		<tr>
			<td rowspan="3" align="center"><strong>Menambah Data Barang</strong></td>
			<td>Mengisi form data barang sesuai dengan kebutuhan sistem</td>
			<td>SRS-2.2.8</td>
			<td>STD-3.0</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Mengosongkan form input data barang</td>
			<td>SRS-2.2.8</td>
			<td>STD-3.1</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Tidak terkoneksi dengan internet</td>
			<td>SRS-2.2.8</td>
			<td>STD-3.2</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
        <!-- Scan QR Code / transaksi --> 
		<tr>
			<td rowspan="3" align="center"><strong>Scan QR Code</strong></td>
			<td>Member melakukan scan QR Code yang berisi kode barang dari toko</td>
			<td>SRS-2.2.2</td>
			<td>STD-4.0</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Member melakukan scan QR Code yang berisi bukan kode barang dari toko</td>
			<td>SRS-2.2.2</td>
			<td>STD-4.1</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
		<tr>
			<td>Tidak terkoneksi dengan internet</td>
			<td>SRS-2.2.2</td>
			<td>STD-4.2</td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Luqman</td>
		</tr>
        <!-- <! Login User Web Pemilik Toko > -->
		<tr>
			<td rowspan="3" align="center"><strong>Login User Pemilik Toko</strong></td>
			<td>Username dan Password yang di masukkan sesuai data yang ada pada database</td>
			<td> SRS-2.2.9 </td>
			<td> STD-5.0 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<tr>
			<td>Username dan Password yang di masukkan tidak sesuai data yang ada pada database</td>
			<td> SRS-2.2.9 </td>
			<td> STD-5.1 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td> 
		</tr>
		<tr>
			<td>Tidak mengisi form login </td>
			<td> SRS-2.2.9 </td>
			<td> STD-5.2 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<!-- Input Data Karyawan Pada Web Toko --> 
		<tr>
			<td rowspan="3" align="center"><strong>Menambah Data Karyawan Web Toko</strong></td>
			<td>Mengisi form data Karyawan sesuai dengan kebutuhan sistem</td>
			<td> SRS-2.2.11 </td>
			<td> STD-6.0 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<tr>
			<td>Mengosongkan kolom pada form input data Karwayan</td>
			<td> SRS-2.2.11 </td>
			<td> STD-6.1 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<tr>
			<td>Memasukan Alamat email tanpa '@' pada kolom input data karyawan</td>
			<td> SRS-2.2.11 </td>
			<td> STD-6.2 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<!-- Input Data Pemasok Pada Web Toko --> 
		<tr>
			<td rowspan="3" align="center"><strong>Menambah Data Pemasok Web Toko</strong></td>
			<td>Mengisi form data Pemasok sesuai dengan kebutuhan sistem</td>
			<td> - </td>
			<td> STD-7.0 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<tr>
			<td>Mengosongkan salah satu kolom pada form input data Pemasok</td>
			<td> - </td>
			<td> STD-7.1 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
		<tr>
			<td>Memasukan Nama yang sama pada kolom input data Pemasok</td>
			<td> - </td>
			<td> STD-7.2 </td>
			<td>sistem</td>
			<td>Black Box</td>
			<td>Mochamad Faizal</td>
		</tr>
	</thead>
</table>

##
### BAB 4 Deskripsi dan Hasil Uji

<!-- Login User sesuai data-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-1.0</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Username dan Password sesuai data yang ada pada database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login berhasil masuk ke halaman dashboard user</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Username dan password yang sesuai database <br>
					 klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Username  : luqman <br>
					 Password  : luqman
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User dapat login dengan data yang sesuai dan masuk ke halaman dashboard user
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Username dan password harus sesuai dengan database.
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Login User tidak sesuai database-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-1.1</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Username dan Password tidak sesuai data yang ada pada databse</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login dengan data yang salah akan berhasil masuk ke halaman dashboard user</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Username dan password yang tidak sesuai database <br>
					 klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 user name : luqman <br>
					 Password  : hakim
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat login dengan data yang tidak sesuai dan tidak dapat masuk ke halaman dashboard user
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Username dan password yang tidak sesuai dengan data tidak dapat login dan user tidak dapat masuk ke halaman dashboard user
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Login User dengan data kosong-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-1.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Tidak mengisi Username dan Password </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login berhasil jika tidak mengisi form login</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Tidak menginputkan apapun pada form login <br>
					 klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 tidak ada
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat login karena tidak mengisi form login
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa form harus diisi
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Register member sesuai requirement-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-2.0</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengisi form register sesuai dengan data yang diminta sistem</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Register berhasil dan data dapat masuk ke dalam database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Register<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama, Alamat, No Hp, Email, Username dan Password sesuai dengan yang diminta sistem <br>
					 klik tombol daftar
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama  : luqmanul Hakim <br>
					 Alamat  : indramayu <br>
					 No HP  : 083824397272 <br>
					 Email  : luqmanulhakim0422978@gmail.com <br>
					 Username  : luqman <br>
					 Password  : luqman
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Member dapat mendaftarkan diri dengan data yang telah di inputkan dan datanya tersimpan ke database
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Data yang di inputkan harus dengan format yang sesuai dengan form register
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Register Member tidak mengisi form register-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-2.1</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Tidak mengisi form register</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Register dapat dilakukan dengan form register yang kosong atau tidak diisi</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Register<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Tidak menginputkan data apapun pada form register <br>
					 klik tombol daftar
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 tidak ada
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat register karena tidak ada data yang diinputkan 
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa kolom tidak boleh ada yang kosong
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Register Member dengan data yang tidak valid-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-2.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengisi email tidak sesuai dengan format yang diminta sistem (kurang karakter '@') </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Register berhasil dengan inputan email yang tidak sesuai dengan kebutuhan sistem</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Register<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama, Alamat, No Hp, Email tanpa karakter '@', Username dan Password <br>
					 klik tombol daftar
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama  : luqmanul Hakim <br>
					 Alamat  : indramayu <br>
					 No HP  : 083824397272 <br>
					 Email  : luqmanulhakim <br>
					 Username  : luqman <br>
					 Password  : luqman
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat register karena email yang di inputkan tidak sesuai dengan data yang dibutuhkan sistem (dalam kasus ini kurang karakter '@')
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa email yang diinput harus valid yaitu disertai dengan karakter '@'
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Input Data Barang Sesuai Requierement-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-3.0</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengisi form input barang sesuai dengan data yang diminta sistem</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Tambah data barang berhasil dan data dapat masuk ke dalam database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Barang<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama Barang, Harga beli, Harga jual, Satuan, dan Stok sesuai dengan yang diminta sistem <br>
					 klik tombol tambah
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama Barang  : Krupuk <br>
					 Harga beli  : 3000 <br>
					 Harga jual  : 5000 <br>
					 Satuan  : Pak <br>
					 Stok  : 20
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Data barang dapat masuk ke database dan dapat tampil ke list data barang
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Data yang disimpan dan ditampilkan sama dengan data yang diinput
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Input data barang dengan kolom kosong-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-3.1</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengosongkan form input data barang</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Tambah data dapat dilakukan dengan form input barang yang kosong atau tidak diisi</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Barang<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Tidak menginputkan data apapun pada form input data barang <br>
					 klik tombol tambah
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 tidak ada
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat melakukan input data barang karena tidak ada data yang diinputkan di form input data barang
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa kolom tidak boleh ada yang kosong
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Input Data barang tanpa koneksi internet-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-3.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Tidak terkoneksi dengan internet </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Tambah data barang berhasil tanpa adanya koneksi internet</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Barang<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama Barang, Harga beli, Harga jual, Satuan, dan Stok sesuai dengan yang diminta sistem <br>
					 klik tombol tambah
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama Barang  : Krupuk <br>
					 Harga beli  : 3000 <br>
					 Harga jual  : 5000 <br>
					 Satuan  : Pak <br>
					 Stok  : 20
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Data barang tidak dapat ditambahkan ke dalam database karena aplikasi tidak terkoneksi dengan internet
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa aplikasi tidak terkoneksi ke internet, dan untuk dapat menambahkan data barang aplikasi harus terkoneksi dengan internet
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Scan QR Code -->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-4.0</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Member melakukan scan QR Code yang berisi kode barang dari toko</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa Hasil scan data dari QR Code dan database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Dashboard Member<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Member memilih menu scan pada navbar menu <br>
					 Member mengarahkan kamera tepat ke QR Code
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 QR Code
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Aplikasi dapat membaca QR Code dan menampilkan data barang dari database dalam bentuk menu popup
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     QR Code harus berisi id dari barang yang ada di toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Scan member dari QR Code yang bukan berisi data dari barang di toko-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-4.1</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Member melakukan scan QR Code yang berisi bukan kode barang dari toko</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Scan dapat dilakukan dengan QR Code yang berisi bukan data barang dari toko</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Dashboard Member<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Member memilih menu scan pada navbar menu <br>
					 Member mengarahkan kamera ke QR Code yang bukan dari toko
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 QR Code yang bukan dari toko dan bukan berisi data barang dari toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Scan dapat dilakukan namun tidak menampilkan data barang dan terdapat toast bahwa barang tidak terdapat di toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan data barang tidak ditemukan
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Scan QR Code tanpa koneksi-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-4.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Tidak terkoneksi dengan internet</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Scan berhasil tanpa adanya koneksi internet</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Dashboard Member<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Luqman</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Member memilih menu scan pada navbar menu <br>
					 Member mengarahkan kamera ke QR Code
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 QR Code dari toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Scan gagal dan akan terdapat pemberitahuan tidak terkoneksi dengan internet
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa aplikasi tidak terkoneksi dengan internet
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Login User Pemilik toko dengan data kosong-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3"> 5.0 </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Username dan Password yang di masukkan sesuai data yang ada pada database </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login dengan data yang salah akan berhasil masuk ke halaman dashboard pemilik toko</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Username dan password yang sesuai database <br>
                     klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul>
					 Username  : faizal <br>
					 Password  : faizal
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Pemilik toko dapat login dengan data yang sesuai dan masuk ke halaman dashboard pemilik toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Username dan password harus sesuai dengan database.
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3"> 5.1 </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Username dan Password yang di masukkan tidak sesuai data yang ada pada database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login dengan data yang salah akan berhasil masuk ke halaman dashboard pemilik</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Username dan password yang tidak sesuai database<br>
                     klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Username  : faizal <br>
					 Password  : 12345
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 User tidak dapat login dengan data yang tidak sesuai dan tidak dapat masuk ke halaman dashboard pemilik toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Username dan password yang tidak sesuai dengan data tidak dapat login dan user tidak dapat masuk ke halaman dashboard pemilik toko
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Login Web Pemilik Toko dengan data kosong-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-5.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Tidak mengisi Username dan Password </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Login berhasil jika tidak mengisi form login</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Login<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Tidak menginputkan apapun pada form login <br>
					 klik tombol login
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 tidak ada
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Pemilik Toko tidak dapat login karena tidak mengisi form login
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa form harus diisi
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Register member sesuai requirement-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-6.0</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengisi form data Karyawan sesuai dengan kebutuhan sistem</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Tambah data karyawan berhasil dan data dapat masuk ke dalam database</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Karyawan<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama, Alamat, No Hp, Email, Username dan Password sesuai dengan yang diminta sistem <br>
					 klik tombol tambah
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama  : mochamad faizal <br>
					 Alamat  : indramayu <br>
					 No HP  : 083928772817 <br>
					 Email  : mchfaizal@gmail.com <br>
					 Username  : faizal <br>
					 Password  : faizal
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Pemilik toko dapat menambahkan data karyawan dan datanya tersimpan ke database
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Data yang di inputkan harus dengan format yang sesuai dengan form tambah data karyawan
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
<!-- Register Member tidak mengisi form register-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-6.1</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Mengosongkan kolom pada form input data Karwayan</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah tambah data karyawan dapat dilakukan dengan form data karyawan yang kosong atau tidak diisi</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Karyawan<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Tidak menginputkan data apapun pada form data karyawan <br>
					 klik tombol tambah
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 tidak ada
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Pemilik toko tidak dapat menambah data karyawan karena tidak ada data yang diinputkan 
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa kolom tidak boleh ada yang kosong
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>

<!-- Register Member dengan data yang tidak valid-->
<table>  
	<thead> 
		<tr>
			<td rowspan="1"><strong>Identifikasi</td>
			<td colspan="3">STD-6.2</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Nama Butir Uji</td>
			<td colspan="3">Memasukan Alamat email tanpa '@' pada kolom input data karyawan </td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tujuan</td>
			<td colspan="3">Memeriksa apakah Input data karyawan berhasil dengan inputan email yang tidak sesuai dengan kebutuhan sistem</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Kondisi Awal</td>
			<td colspan="3">Halaman Input Data Karyawan<br>
			</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Tanggal Pengujian</td>
			<td colspan="3">20-05-2018</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Penguji</td>
			<td colspan="3">Mochamad Faizal</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Skenario</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>
					 Input Nama, Alamat, No Hp, Email tanpa karakter '@', Username dan Password <br>
					 klik tombol daftar
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Hasil</td>
		</tr>
		<tr>
			<td rowspan="1"><strong>Data yang Diberikan</td>
			<td rowspan="1"><strong>Yang Diharapkan</td>
			<td rowspan="1"><strong>Pengamatan</td>
			<td rowspan="1"><strong>Kesimpulan</td>
		</tr>
		<tr>
			<td rowspan="1">
				<ul> 
					 Nama  : mochamad faizal <br>
					 Alamat  : indramayu <br>
					 No HP  : 083928772817 <br>
					 Email  : mchfaizal <br>
					 Username  : faizal <br>
					 Password  : faizal
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 Pemilik toko tidak dapat melakukan tambah data karyawan karena email yang di inputkan tidak sesuai dengan data yang dibutuhkan sistem (dalam kasus ini kurang karakter '@')
				</ul>
			</td>
			<td rowspan="1">
				<ul>
				     Terdapat peringatan bahwa email yang diinput harus valid yaitu disertai dengan karakter '@'
				</ul>
			</td>
			<td rowspan="1">
				<ul>
					 OK
				</ul>
			</td>
		</tr>
		<tr>
			<td colspan="4" align="center"><strong>Catatan</td>
		</tr>
		<tr>
			<td colspan="4">
				<ul>					
				</ul>
			</td>
		</tr>
	</thead>
</table>
