<html>
<body>
<h1><p align="center">Software Requirements Spesification</p></h1>

<p align="center"><b>Version 2.0.1 </b><br>
<p align="center">13 April 2018</b><br><br>
<p align="center">
<img src="http://i67.tinypic.com/2yuhmww.png"/>
</p>

<br><p align="center"><b> APLIKASI POS QR-CODE ANDROID</b><br>
<p align="center"><b>Aplikasi Menggunakan Kode QR
</b>
<p align="center">Kelompok 2<br>
 Mochamad Faizal 			(1603179)<br>
 Luqmanul Hakim				(1603076)<br>
 Inneke Widianti			(1603072)<br>
 Rizaluddin Sidqi Baihaqi	(1603082)<br><br><br>

<p align="center"><b>Jurusan Teknik Informatika</b><br>
<p align="center"><b>Politeknik Negeri Indramayu</b><br>
</p>
</body>
</html>

##

### BAB I Pendahuluan
Dokumen ini berisi penjelasan pemakaian dan penulisan dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) atau Software Requirement Specification (SRS). Dokumen ini selanjutnya akan menggunakan istilah SRS.

Software Requirement Specification (SRS) menjelaskan berbagai macam kebutuhan pembuatan produk, yaitu kebutuhan spesifik yang terdiri dari kebutuhan fungsionalitas, termasukdidalamnya input, proses, dan output dari produk dan non-fungsionalitas. Kebutuhan antar muka juga digambarkan dengan jelas di dalam dokumen ini, terdiri dari kebutuhan antar pengguna, antar hardware yang menjelaskan kebutuhan yang harus ada untuk menjalankan atau mengoperasikan aplikasi sistem, kebutuhan antar software yang menjelaskan bagaimana cara pengguna berinteraksi dengan sistem, dan kebutuhan antar komunikasi.

Dokumen ini dibuat untuk membantu membuat spesifikasi perangkat lunak yang akan dikembangkan dengan rancangan berorientasi proses. Pada prinsipnya, hasil analisis sistem perangkat lunak dengan rancangan ini diuraikan sebagai sekumpulan proses yang terorganisasi secara hirarkis, memberikan solusi, batasan masalah agar proyek tidak menyimpang terlalu jauh dari tujuan awal, dan manfaat dari sistem informasi yang akan dibuat. Software Requirement Spesification ini dapat dijadikan acuan agar proyek dapat berjalan dengan lancar selama pengerjaannya.

__1.1 Tujuan__
<br>Tujuan dari dokumen Software Requirement Specification (SRS) ini adalah memberikan gambaran yang spesifik dari kebutuhan software. Spesifikasi kebutuhan tersebut termasuk dari segi perangkat lunak dan perangkat keras, untuk memberikan gambaran dan penjelasan mengenai pembuatan produk, penjelasan hal-hal yang dibutuhkan untuk pembuatan produk termasuk kebutuhan fungsional hingga nonfungsional, dan kebutuhan antar muka mulai dari antar muka pengguna hingga antar muka komunikasi.

__1.2 Lingkup__
<br>Semua hal yang tercantum didalam dokumen ini merupakan bagian dari ruang lingkup kebutuhan pembangunan perangkat lunak yang berupa aplikasi kasir QR Code berbasis android yang digunakan untuk perhitugan keuangan pada toko-toko.

__1.3 Definisi, Akronim dan Singkatan__
<br>

Definisi, Akronim dan Singkatan | Penjelasan |
-----------------|---------------------------
SRS/SKPL | adalah dokumen yang menggambarkan secara detail spesifikasi kebutuhan software dalam pembangunan proyek perangkat lunak Aplikasi Kasir QR Code Berbasis Android.|
DFD | adalah suatu diagram yang menggunakan notasi-notasi untuk menggambarkan arus dari data pada suatu sistem atau menjelaskan proses kerja suatu sistem, yang penggunaannya sangat membantu untuk memahami sistem secara logika, tersruktur dan jelas.|
Software | Perangkat Lunak.|
Hardware | Perangkat Keras|
SRS | Software Requirements Specification.|
SKPL | Spesifikasi Kebutuhan Perangkat Lunak.|
DFD | Data Flow Diagram|
IEEE | The Institute of Electrical and Electronics Engineers|

__1.4 References__
- IEEE Std. 830-1998, IEEE Recommended Practice for Software Requirement Specifications.

__1.5 Overview__
<br>Dokumen SRS ini merupakan acuan untuk mengetahui spesifikasi kebutuhan dalam menyelesaikan proyek ini. Dokumen SRS ini berisi tentang deskripsi tentang kebutuhan perangkat lunak (tools pendukung, peranangan sistem yang akan dikembangkan), perangkat keras, dan sumber daya manusia (SDM).

##
 
### BAB II GAMBARAN UMUM
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

__2.1 Perspektif produk__
<br>Aplikasi point of sales dengan QR-Code berbasis android adalah sebuah sistem transaksi pembayaran yang diaplikaskan pada android. Dimana user dari aplikasi ini pembeli, kasir/karyawan, pemilik toko sedangkan untuk pengolahan datanya dikelola oleh admin yang menggunakan sistem web.

Pada sisem QR Kode mengunakan dara tiap jenia makanan yang dijual ditoko. Data tersebut di enkripsi menjadi sebuah kode QR. kode tersebut akan ditempel pada setiap baris pada jenis makanan yang ada di toko, tujuannya agar pembeli dapat dengan mudah melakukan scan untuk melihat harga pada tiap makanan atau membelinya dengan cara melakukan scan terlebih dahulu. Sebelum pembeli menggunakan aplikasi ini, pembeli diwajibkan mendaftar dengan imek hanphone masing-masing dan nomor handphone tersebut.

Pada sistem pembeli, dapat melakukan scan QR pada tiap-tiap jenis makanan yang ditoko, dan membeli dengan jumlah yang di inginkan, setelah melakukan pembelian, makanan dicek dikasir untuk dicocokan dengan data yang ada pada aplikasi, jika data dana barang sudah benar, lalu penghitungan, setelah pembayaran, struk digital pun langsung dikirim pada aplikasi pembeli. Pada sistem kasir/karyawan, dapat melihat makanan apa saja yang pembeli beli,lalu dihitung.

____2.1.1 Antarmuka sistem____

![Antarmuka Sistem](http://i63.tinypic.com/ri9ouf.jpg)

Aplikasi POS Dengan QR Code scanner ini mempunyai 4 user yaitu Admin, Pemilik Toko, Karyawan dan Member. Dalam aplikasinya terdapat 2 fungsi utama yaitu melakukan pengolahan data dan transaksi. Admin memiliki fungsi mengelola data yang ada pada aplikasi seperti data toko, karyawan, dan juga member. Pemilik toko memiliki fungsi untuk mengelola segala data yang berhubungan dengan toko yang dimilikinya, seperti data karyawan, data barang dan data laporan transaksi. Karyawan mempunyai fungsi untuk mengelola data barang dan melakukan transaksi. Member mempunyai fungsi Transaksi dengan cara melakukan scan dan juga melakukan pembayaran baik secara cash ataupun dengan e-payment.

____2.1.2 Antarmuka pengguna____

- Mock up android

<div>
	<table>
		<tr align="center">
			<td><b>Icon Aplikasi</b></td>
			<td><b>Splashscreen</b></td>
			<td width="300"><b>Sign In</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/30cyg7q.png" width="180" height="350" /><br><p align="justify">Ini adalah tampilan ikon aplikasi Q-Pay pada menu di Smartphone.</p></td>
				<td><img src="http://i65.tinypic.com/k48ms7.png" width="180" height="350" /><br><p align="justify">Splashscreen adalah tampilan awal saat aplikasi dibuka, pada aplikasi kami tampilan awalnya beupa logo dan nama aplikasi.</p></td>
				<td><img src="http://i64.tinypic.com/rr73uh.png" width="180" height="350" /><br><p align="justify">Pada tampilan sign in ini user akan memasukkan username dan password untuk bisa masuk ke tampilan dashboard, pada platform android terdapat  2 user yaitu member dan karyawan, kemudian setelah berhasil login akan secara otomatis diarahkan ke menu dari masing-masing user.</p></td>		
		</tr>
		<tr align="center">
			<td><b>Sign Up</td>
			<td><b>Dashboard Member</td>
			<td><b>Navbar Menu</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i64.tinypic.com/554ax0.png" width="180" height="350" /><br><p align="justify">Tampilan Sign Up ini adalah tampilan register bagi member yang belum mempunyai akun.</p></td>
				<td><img src="http://i63.tinypic.com/2u6k4js.png" width="180" height="350" /><br><p align="justify">Pada tampilan Dashboard member ini terdapat tampilan utama yang berisi foto-foto dan promo toko.</p></td>
				<td><img src="http://i65.tinypic.com/20itelf.png" width="180" height="350" /><br><p align="justify">Pada tampilan Navbar ini tersedia menu-menu untuk member seperti scan, daftar belanja, topup, struk, setting dan lainnya.</p></td>		
		</tr>
		<tr align="center">
			<td><b>Scan</td>
			<td><b>Hasil Scan</td>
			<td><b>Daftar belanja</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i68.tinypic.com/eb6649.png" width="180" height="350" /><br><p align="justify">Pada tampilan scan ini member akan melakukan scan pada QR Code yang ditempel pada rak produk menggunakan menu scan dari aplikasi Q-pay</p></td>
				<td><img src="http://i63.tinypic.com/m75qom.png" width="180" height="350" /><br><p align="justify">Pada tampilan hasil scan akan muncul tampilan berupa pop up dimana akan ditampilkan nama produk dan juga harga produk, kemudian member diminta untuk memasukkan jumlah produk jika ingin melanjutkan pembelian.</p></td>
				<td><img src="http://i67.tinypic.com/2aeyud1.png" width="180" height="350" /><br><p align="justify">Pada menu daftar belanja ini akan tampil list produk yang sudah di scan beserta keterangan harga masing-masing produk dan total harga yang harus dibayar.</p></td>		
		</tr>
		<tr align="center">
			<td><b>Struk</td>
			<td><b>Detail Struk</td>
			<td><b>Dashboard Karyawan</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i68.tinypic.com/2hx7tr9.png" width="180" height="350" /><br><p align="justify">Pada menu struk ini akan ditampilkan list dari struk transaksi yang pernah dilakukan member di toko tersebut beserta dengan tanggal transaksinya.</p></td>
				<td><img src="http://i64.tinypic.com/334p8ie.png" width="180" height="350" /><br><p align="justify">Padaq tampilan detail struk ini akan ditampilkan rincian dari produk, harga, beserta total harga dari transaksi yang pernah dilakukan member.</p></td>
				<td><img src="http://i67.tinypic.com/34j3fyc.png" width="180" height="350" /><br><p align="justify">Dashboard karyawan ini merupakan menu utama dari user karyawan dimana akan ditampilkan nama karyawan yang telah login.</p></td>		
		</tr>
		<tr align="center">
            <td> <b>Navbar Karyawan</td>
			<td> <b>Data Barang</td>
		</tr>
		<tr valign="top" align="center">
            <td><img src="http://i64.tinypic.com/xlbk06.png" width="180" height="350" /><br><p align="justify">Pada tampilan navbar karyawan ini terdapat menu-menu yang bisa digunakan oleh user karyawan diantaranya menu data barang dan menu transaksi.</p></td>
			<td><img src="http://i68.tinypic.com/wcl84j.png" width="180" height="350" /><br><p align="justify">Pada menu data barang ini karyawan dapat mengelola data barang seperti menambahkan barang, mengubah data barang, menghapus data barang dan melihat data barang.</p></td>
		</tr>
	</table>
    </div>

- Mock up web
	<table>
		<tr align="center">
			<td><b>Dashboard Pemilik Toko</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i63.tinypic.com/15i0l6g.png" /><br><p align="justify">Ini adalah tampilan dashboard untuk user pemilik toko yang berisi tampilan data umum dan menu-menu untuk pemilik toko.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Side Menu Master</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i64.tinypic.com/1dzih3.png" /><br><p align="justify">Ini adalah tampilan side menu dari menu master, dimana didalamnya terdapat submenu data karyawan, data pemasok, dan data toko.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Side Menu Transaksi</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i63.tinypic.com/314a59l.png" /><br><p align="justify">Ini adalah tampilan side menu dari menu transaksi, dimana didalamnya terdapat submenu data penjualan, dan data pembelian.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Side Menu Laporan</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/314r1qb.png" /><br><p align="justify">Ini adalah tampilan side menu dari menu laporan, dimana didalamnya terdapat submenu laporan stock, laporan penjualan, dan laporan pembelian.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Tambah Karyawan</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i67.tinypic.com/34hf3ts.png" /><br><p align="justify">Ini adalah tampilan tambah data karyawan yang berisi form data yang dibutuhkan untuk menambahkan karyawan.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Data Karyawan</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i64.tinypic.com/1zlsqjr.png" /><br><p align="justify">Ini adalah tampilan data karyawan yang berisi list karyawan beserta datanya yang sudah ditambahkan oleh pemilik toko.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Data Pemasok</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/aob8t3.png" /><br><p align="justify">Ini adalah tampilan data pemasok yang memberikan supply produk untuk pemilik toko, tampilannya berisi list pemasok beserta dengan datanya.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Tambah Data Pemasok</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i63.tinypic.com/beiqfb.png" /><br><p align="justify">Ini adalah tampilan tambah data pemasok yang berisi form data yang dibutuhkan untuk menambahkan pemasok.</p></td>	
		</tr>
		</table>



   
____2.1.3 Antarmuka perangkat keras____
<br>Kebutuhan minimum perangkat keras yang dapat digunakan oleh aplikasi ini adalah :

<br>- Smarthpone Android
<br>Dibutuhkan sebuah smartphone dengan os Android yang dilengkapi dengan kamera untuk dapat menggunakan aplikasi Q-Pay ini untuk user member dan user karyawan.

<br>- PC/Laptop
<br>Untuk admin dan pemilik toko membutuhkan PC/Laptop untuk dapat menggunakan aplikasi Q-Pay ini.



![use case 1](http://i63.tinypic.com/2na8rxe.jpg)

____2.1.4 Antarmuka perangkat lunak____
<br>Perangkat lunak yang dibutuhkan untuk aplikasi ini yaitu :
<ul>
<li>Android Studio</li>
<li>Sublime Teks</li>
<li>XAMPP</li>
<li>Balsamiq Mockup3</li>
</ul>

____2.1.5 Antarmuka komunikasi____
<br>Yang dibutuhkan hanya sebuah android dan pc yang dapat terhubung ke internet.

____2.1.6 Batasan-batasan memori____
<br>Perangkat lunak hanya dapat dijalankan di android.

____2.1.7 Operasi-operasi____

|Operasi|Fungsi  |
|--|--|
|Sign Up Member|Digunakan member untuk mendaftar ke aplikasi|
|Sign Up Toko|Digunakan pemilik toko untuk mendaftarkan toko mereka|
|Login|Digunakan untuk masuk akses aplikasi|
|Tambah Karyawan|Digunakan pemilik toko untuk menambahkan karyawan|
|Tambah Barang|Digunakan karyawan atau pemilik toko untuk menambahkan barang|
|Scan|Digunakan untuk membaca QR Code pada barang|
|Topup|Digunakan member untuk melakukan pembayaran dengan tabungan|
|Cari Barang|Digunakan untuk mencari barang|
|Cari Karyawan|Digunakan untuk mencari karyawan|
|Cari Toko|Digunakan untuk mencari toko|
|Pilih Toko|Digunakan untuk memilih toko tempat transaksi|
|Struk|Digunakan untuk menampilkan list struk dari transaksi member|
|Cetak Struk|Digunakan karyawan untuk mencetak struk ke sisi member|
|Detail Struk|Digunakan untuk memberikan detail struk transaksi|
|Kembali|Digunakan untuk kembali ke halaman sebelumnya|
|Hapus|Digunakan untuk menghapus data|
|Edit|Digunakan untuk mengedit data|
|Simpan|Digunakan untuk menyimpan data|
|Download Laporan|Digunakan untuk mendownload file laporan penjualan|

____2.1.8 Kebutuhan-kebutuhan dalam tahapan adaptasi____

__2.2 Spesifikasi Kebutuhan Fungsional__

![use case 2](http://i65.tinypic.com/2m29wsw.jpg)

![use case 3](http://i63.tinypic.com/2agp6br.jpg)

__2.2.1 Sign Up dan Login Member__

![Login Member](http://i63.tinypic.com/2m7698n.jpg)

Untuk dapat menggunakan aplikasi member harus mengisi form login terlebih dahulu  dengan cara:
<br>1. Member mengaktifkan fungsi login
<br>2. Sistem menampilkan halaman login yang terdiri dari email dan password
<br>3. Member mengisi email dan password
<br>4. Sistem melakukan validasi dari email dan password
<br>5. Jika login gagal maka member akan diminta mengulangi proses login
<br>6. Jika login berhasil maka member akan diarahkan ke halaman pilih toko

Untuk member yang belum mempunyai akun diharuskan melakukan sign up terlebih dahulu dengan cara:
<br>1.Member mangaktifkan fungsi sign up
<br>2. Sistem menampilkan halaman register
<br>3. Member mengisi form register sesuai dengan yang ditampilkan sistem
<br>4. Sistem menyimpan data yang dimasukkan member

__2.2.2 Scan Member__

![Scan Member](http://i63.tinypic.com/157ya9l.jpg)

Member harus melakukan scan untuk mengetahui harga produk dan memasukkannya ke daftar belanjaan dengan cara :

<br>1. Member mengaktifkan menu scan
<br>2. Sistem mengaktifkan kamera smartphone
<br>3. Member mengarahkan kamera ke QR Code yang ada pada rak produk
<br>4. Sistem membaca dan menerjemahkan QR Code
<br>5. Sistem menampilkan harga dari produk
<br>6. Member memasukkan pilihan untuk melanjutkan

__2.2.3 Total Harga Member__

![Scan Member](http://i68.tinypic.com/2j4d4pt.jpg)

Member dapat melihat total harga dan data belanjaan yang sudah diambil dan akan dibayar, dengan cara :

1.Member masuk ke main menu
<br>2.Sistem menampilkan pilihan menu
<br>3.Member memilih menu daftar belanja

__2.2.4 Total Harga Member__

![](http://i68.tinypic.com/23vko6s.jpg)

Member dapat melakukan transaksi atau pembayaran secara manual ataupun menggunakan top up, dengan cara :

1.Member masuk ke main menu
<br>2.Sistem menampilkan pilihan menu
<br>3.Member memilih menu daftar belanja
<br>4.Member memberikan input oke untuk melanjutkan ke fungsi transaksi
<br>5.Sistem menampilkan pilihan pemmbayaran
<br>6.Jika member memilih pembayaran manual, member dapat langsung membayar ke kasir
<br>7.Jika user memilih menggunakan top up/e-cash maka sistem akan mengecek data saldo member
<br>8.Jika saldo mencukupi untuk membayar belanjaan maka saldo akan langsung diambil sesuai harga belanjaan
<br>9.Jika saldo tidak mencukupi maka member harus membayar secara manual 

__2.2.5 Login Karyawan__

![](http://i66.tinypic.com/1z3nu6r.jpg)

Untuk dapat menggunakan aplikasi karyawan harus mengisi form login terlebih dahulu  dengan cara:

1.Karyawan mengaktifkan fungsi login
<br>2.Sistem menampilkan halaman login yang terdiri dari email dan password
<br>3.Karyawan mengisi email dan password yang sudah diberikan oleh pemilik toko
<br>4.Sistem melakukan validasi dari email dan password
<br>5.Jika login gagal maka karyawan akan diminta mengulangi proses login
<br>6.Jika login berhasil maka karyawan akan diarahkan ke halaman dashboard karyawan

__2.2.6 Terima List Belanja Karyawan__

![](http://i66.tinypic.com/103txyx.jpg)

Karyawan akan dapat melihat list belanja dari member, dengan cara:

1.Karyawan mengaktifkan fungsi transaksi
<br>2.Sistem menampilkan data member yang sudah mengirimkan data belanja
<br>3.Karyawan memilih data member yang ingin dilihat
<br>4.Sistem menampilkan list belanjaan dari member yang telah dipilih oleh karyawan

__2.2.7 Transaksi Karyawan__

![](http://i64.tinypic.com/21n4acn.jpg)

Karyawan akan dapat melakukan transaksi dengan member, dengan cara:

1.Karyawan mengaktifkan fungsi transaksi
<br>2.Sistem menampilkan data member yang sudah mengirimkan data belanja
<br>3.Karyawan memilih data member yang ingin dilihat
<br>4.Sistem menampilkan list belanjaan dari member yang telah dipilih oleh karyawan
<br>5.Jika member memilih membayar secara manual maka kasir menginputkan uang yang dibayarkan oleh member
<br>6.Jika member memilih pembayaran dengan top up maka karyawan langsung melakukan cetak struk dengan menekan tombol cetak struk

__2.2.8 Input data barang Karyawan__

![](http://i66.tinypic.com/ayaj5h.jpg)

Karyawan akan dapat melakukan input barang, dengan cara:

1.Karyawan mengaktifkan fungsi data barang
<br>2.Sistem menampilkan data barang yang sudah ada
<br>3.Karyawan menekan tombol icon tambah
<br>4.Sistem menampilkan form input barang
<br>5.Karyawan mengisi form sesuai dengan requirement
<br>6.Sistem akan melakukan validasi
<br>7.Sistem menyimpan data barang ke dalam database

__2.2.9 Sign Up Toko__

![](http://i64.tinypic.com/16ln1wi.jpg)

Pemilik toko harus mendaftarkan tokonya terlebih dahulu untuk dapat menggunakan aplikasi kami, dengan cara:

1.Pemilik toko mengakses web aplikasi Q-pay
<br>2.Pemilik toko memilih menu daftar toko
<br>3.Sistem menampilkan form pendaftaran toko
<br>4.Pemilik toko mengisi form pendaftaran
<br>5.Pemilik toko menekan tombol daftar
<br>6.Sistem akan melakukan validasi
<br>7.Sistem menyimpan data toko ke dalam database

Kemudian setelah sign up maka pemilik toko diharuskan login, dengan cara :

1.Pemilik toko mengakses web aplikasi Q-pay
<br>2.Pemilik toko memilih menu login
<br>3.Sistem menampilkan form login
<br>4.Pemilik toko mengisi form login
<br>5.Pemilik toko menekan tombol login
<br>6.Sistem akan melakukan validasi dari username dan password
<br>7.Jika username dan password sesuai maka sistem akan menampilkan dashboard pemilik toko
<br>8.Jika username dan password tidak sesuai maka sistem akan meminta pemilik toko untuk mengisi ulang form login

__2.3.0 Lihat laporan penjualan__

![](http://i65.tinypic.com/32zt7at.jpg)

Pemilik toko dapat melihat laporan dari penjualan toko mereka melalui aplikasi kami, dengan cara:

1.Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2.Sistem menampilkan menu untuk pemilik toko
<br>3.Pemilik toko memilih menu laporan penjualan
<br>4.Sistem menampilkan laporan penjualan

__2.3.1 Daftar karyawan__

![](http://i63.tinypic.com/24v4ht4.jpg)

Pemilik toko dapat mendaftarkan atau menambah karyawan toko mereka, dengan cara:

1.Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2.Sistem menampilkan menu untuk pemilik toko
<br>3.Pemilik toko memilih menu tambah karyawan
<br>4.Sistem menampilkan form penambahan karyawan
<br>5.Pemilik toko mengisi form penambahan karayawan
<br>6.Sistem menyimpan data karyawan ke dalam database

__2.3.2 Tarik uang__

![](http://i64.tinypic.com/16ih2j9.jpg)

Pemilik toko dapat mencairkan saldo bagi pembelian produk dengan pembayaran menggunakan e-cash atau top up, dengan cara:

__2.3.3 Input data barang__

![](http://i66.tinypic.com/2jcbhuc.jpg)

Pemilik toko dapat mennambahkan data barang, dengan cara:

1.Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2.Sistem menampilkan menu untuk pemilik toko
<br>3.Pemilik toko memilih menu tambah karyawan
<br>4.Sistem menampilkan form penambahan karyawan
<br>5.Pemilik toko mengisi form penambahan karayawan
<br>6.Sistem menyimpan data karyawan ke dalam database


__2.3 Spesifikasi Kebutuhan Non-Fungsional__

__2.4 Karakteristik pengguna__

__2.5 Batasan-batasan__

__2.6 Asumsi-asumsi keterkaitan__

__2.7 Kebutuhan penyeimbang__


## BAB III KEBUTUHAN LAIN YANG SPESIFIK
Kebutuhan fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input, proses dan output. Kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan ini yaitu sistem harus dapat mempermudah pengguna dalam menggunkan aplikasi ini.


## BAB IV INFORMASI PENDUKUNG
![](http://i64.tinypic.com/jz8qh2.jpg)
