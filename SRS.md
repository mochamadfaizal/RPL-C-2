<html>
<body>
<h1><p align="center">Software Requirements Spesification</p></h1>

<p align="center"><b>Version 2.0.6 </b><br>
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
				<td><img src="http://i66.tinypic.com/2r1zrlv.png" width="180" height="350" /><br><p align="justify">Tampilan Sign Up ini adalah tampilan register bagi member yang belum mempunyai akun.</p></td>
				<td><img src="http://i63.tinypic.com/2u6k4js.png" width="180" height="350" /><br><p align="justify">Pada tampilan Dashboard member ini terdapat tampilan utama yang berisi foto-foto dan promo toko.</p></td>
				<td><img src="http://i66.tinypic.com/2lszc6h.png" width="180" height="350" /><br><p align="justify">Pada tampilan Navbar ini tersedia menu-menu untuk member seperti scan, daftar belanja, topup, struk, setting dan lainnya.</p></td>		
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
			<td><b>Top Up</td>
			<td><b>Isi Saldo</td>
			<td><b>Info transfer</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i68.tinypic.com/20tldug.png" width="180" height="350" /><br><p align="justify">Pada tampilan ini member dapat mengambil saldo dari admin untuk pembayaran dengan memasukkan kode top up</p></td>
				<td><img src="http://i64.tinypic.com/344wehc.png" width="180" height="350" /><br><p align="justify">Pada tampilan ini member dapat mengisi saldo sesuai dengan menu yang tersedia.</p></td>
				<td><img src="http://i67.tinypic.com/2a7bipg.png" width="180" height="350" /><br><p align="justify">Pada menu ini setelah member mengisi menu isi saldo akan ada info member harus mentransfer ke rekening milik admin.</p></td>		
		</tr>
		<tr align="center">
			<td><b>lupa password</td>
			<td><b>Setting Profil</td>
			<td><b>Setting foto profil</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i66.tinypic.com/wi2135.png" width="180" height="350" /><br><p align="justify">Ini adalah tampilan ketika user lupa password, dimana terdapat inputan email dan kemudian sistem akan mengirim ulang password user ke email yang diinputkan dan email harus sesuai dengan email yang digunakan saat login.</p></td>
				<td><img src="http://i67.tinypic.com/2z5q3qv.png" width="180" height="350" /><br><p align="justify">Pada tampilan profil ini akan ditampilkan info profil dari member dan member juga dapa mengubah info profil mereka sendiri.</p></td>
				<td><img src="http://i66.tinypic.com/23vjfkh.png" width="180" height="350" /><br><p align="justify">Pada tampilan ini member dapat mengubah foto profil mereka, bisa dengan foto langsung, mengambil dari galeri atau pun dari folder tertentu pada device</p></td>		
		</tr>
        <tr align="center">
			<td><b>Struk</td>
			<td><b>Detail Struk</td>
			<td><b>Dashboard Karyawan</td>
		</tr>
		<tr valign="top" align="center">
				<td><img src="http://i68.tinypic.com/2hx7tr9.png" width="180" height="350" /><br><p align="justify">Pada menu struk ini akan ditampilkan list dari struk transaksi yang pernah dilakukan member di toko tersebut beserta dengan tanggal transaksinya.</p></td>
				<td><img src="http://i64.tinypic.com/334p8ie.png" width="180" height="350" /><br><p align="justify">Pada tampilan detail struk ini akan ditampilkan rincian dari produk, harga, beserta total harga dari transaksi yang pernah dilakukan member.</p></td>
				<td><img src="http://i67.tinypic.com/34j3fyc.png" width="180" height="350" /><br><p align="justify">Dashboard karyawan ini merupakan menu utama dari user karyawan dimana akan ditampilkan nama karyawan yang telah login.</p></td>		
		</tr>
		<tr align="center">
            <td> <b>Navbar Karyawan</td>
            <td> <b>Navbar Karyawan Transaksi</td>
			<td> <b>Data Barang</td>
		</tr>
		<tr valign="top" align="center">
            <td><img src="http://i63.tinypic.com/95rfpy.png" width="180" height="350" /><br><p align="justify">Pada tampilan navbar karyawan ini terdapat menu-menu yang bisa digunakan oleh user karyawan diantaranya menu data barang dan menu transaksi.</p></td>
			<td><img src="http://i68.tinypic.com/25swz21.png" width="180" height="350" /><br><p align="justify">Pada tampilan sub navbar transaksi ini terdapat submenu transaksi yaitu transaksi penjualan dan transaksi pembelian.</p></td>
			<td><img src="http://i65.tinypic.com/333dgyo.png" width="180" height="350" /><br><p align="justify">Pada menu data barang ini karyawan dapat mengelola data barang seperti menambahkan barang, mengubah data barang, menghapus data barang dan melihat data barang.</p></td>
		</tr>
		<tr align="center">
            <td> <b>Transaksi Penjualan</td>
            <td> <b>Transaksi Pembelian</td>
			<td> <b>Detail transaksi</td>
		</tr>
		<tr valign="top" align="center">
            <td><img src="http://i67.tinypic.com/2z55gcj.png" width="180" height="350" /><br><p align="justify">Pada tampilan menu transaksi penjualan ini akan ditampilkan list transaksi antara toko dengan member.</p></td>
			<td><img src="http://i64.tinypic.com/213md21.png" width="180" height="350" /><br><p align="justify">Pada tampilan menu transaksi pembelian ini akan ditampilkan list transaksi antara toko dengan pemasok yang melakukan supplay barang.</p></td>
			<td><img src="http://i63.tinypic.com/fkv0gz.png" width="180" height="350" /><br><p align="justify">Pada menu detail transaksi ini  karyawan dapat melihat list barang yang dijual untuk transaksi penjualan ataupun list barang yang dibeli jika transaksi pembelian</p></td>
		</tr>
		<tr align="center">
            <td> <b>Input bayar</td>
            <td> <b>Input data barang</td>
		</tr>
		<tr valign="top" align="center">
            <td><img src="http://i66.tinypic.com/5oh9bl.png" width="180" height="350" /><br><p align="justify">Pada tampilan ini karyawan diminta menginputkan pembayaran apabila transaki dilakukan manual atau tidak menggunakan e-cash atau top up.</p></td>
			<td><img src="http://i64.tinypic.com/v5wqrt.png" width="180" height="350" /><br><p align="justify">Pada tampilan ini karyawan dapat menginputkan data barang sesuai dengan form yang tersedia.</p></td>
		</tr>
	</table>
    </div>

<br>

- Mock up web
	<table>
		<tr align="center">
			<td><b>Dashboard Pemilik Toko</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i63.tinypic.com/15i0l6g.png" /><br><p align="justify">Ini adalah tampilan dashboard untuk user pemilik toko yang berisi tampilan data umum dan menu-menu untuk pemilik toko.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Alert Jika username diklik</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i64.tinypic.com/rt1gdj.png" /><br><p align="justify">Ini adalah tampilan jika icon username diklik yang berisi tampilan data umum pemilik toko dan tombol untuk mengubah password dan juga tombol keluar.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Ganti Password</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/2vxgg7t.png" /><br><p align="justify">Ini adalah tampilan jika tombol ganti password diklik. Disini pemilik toko dapat mengubah passwordnya.</p></td>	
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
		<tr align="center">
			<td><b>Data Toko</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/jsydzp.png" /><br><p align="justify">Ini adalah tampilan data toko yang berisi data-data dari toko yang bersangkutan.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Data Penjualan</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i63.tinypic.com/5o5kaq.png" /><br><p align="justify">Ini adalah tampilan data penjualan yang berisi rincian data penjualan dari toko yang bersangkutan.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Data Pembelian</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i65.tinypic.com/27y1xyc.png" /><br><p align="justify">Ini adalah tampilan data pembelian yang berisi rincian data pembelian dari toko yang bersangkutan.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Login Admin</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/2kkf1h.png" /><br><p align="justify">Ini adalah tampilan login untuk admin.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Dashboard Admin</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/2hr1myv.png" /><br><p align="justify">Ini adalah tampilan dashboard untuk user admin yang berisi tampilan data umum dan menu-menu untuk admin.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Data Pengguna</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i68.tinypic.com/j5wnlx.png" /><br><p align="justify">Ini adalah tampilan data pengguna yang berisi informasi umum pengguna.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Pesan</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i64.tinypic.com/23uq53q.png" /><br><p align="justify">Ini adalah tampilan pesan yang berisi pesan-pesan yang masuk ke admin.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Tambah Toko</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i66.tinypic.com/wb7vc2.png" /><br><p align="justify">Ini adalah tampilan tambah toko yang berisi form untuk menambahkan toko.</p></td>	
		</tr>
		<tr align="center">
			<td><b>Daftar Toko</b></td>
		</tr>
		<tr  valign="top" align="center">
				<td><img src="http://i65.tinypic.com/107ql4z.png" /><br><p align="justify">Ini adalah tampilan daftar toko yang sudah terdaftarkan.</p></td>	
		</tr>
		</table>


____2.1.3 Antarmuka perangkat keras____
<br>Kebutuhan minimum perangkat keras yang dapat digunakan oleh aplikasi ini adalah :
- Smarthpone Android
<br>Dibutuhkan sebuah smartphone dengan os Android yang dilengkapi dengan kamera untuk dapat menggunakan aplikasi Q-Pay ini untuk user member dan user karyawan.
- PC/Laptop
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
<br>Besarnya memory yang dibutuhkan untuk menjalankan aplikasi ini diharapkan tidak melebihi 100MB.

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
<br>Sistem ini sangat bergantung pada lokasi, karena disesuaikan pada lokasi toko yang bersangkutan.

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
<br>1. Member mangaktifkan fungsi sign up
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
<br>1. Member masuk ke main menu
<br>2. Sistem menampilkan pilihan menu
<br>3. Member memilih menu daftar belanja

__2.2.4 Total Harga Member__

![](http://i68.tinypic.com/23vko6s.jpg)

Member dapat melakukan transaksi atau pembayaran secara manual ataupun menggunakan top up, dengan cara :
<br>1. Member masuk ke main menu
<br>2. Sistem menampilkan pilihan menu
<br>3. Member memilih menu daftar belanja
<br>4. Member memberikan input oke untuk melanjutkan ke fungsi transaksi
<br>5. Sistem menampilkan pilihan pemmbayaran
<br>6. Jika member memilih pembayaran manual, member dapat langsung membayar ke kasir
<br>7. Jika user memilih menggunakan top up/e-cash maka sistem akan mengecek data saldo member
<br>8. Jika saldo mencukupi untuk membayar belanjaan maka saldo akan langsung diambil sesuai harga belanjaan
<br>9. Jika saldo tidak mencukupi maka member harus membayar secara manual 

__2.2.5 Login Karyawan__

![](http://i66.tinypic.com/1z3nu6r.jpg)

Untuk dapat menggunakan aplikasi karyawan harus mengisi form login terlebih dahulu  dengan cara:
<br>1. Karyawan mengaktifkan fungsi login
<br>2. Sistem menampilkan halaman login yang terdiri dari email dan password
<br>3. Karyawan mengisi email dan password yang sudah diberikan oleh pemilik toko
<br>4. Sistem melakukan validasi dari email dan password
<br>5. Jika login gagal maka karyawan akan diminta mengulangi proses login
<br>6. Jika login berhasil maka karyawan akan diarahkan ke halaman dashboard karyawan

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
<br>1. Karyawan mengaktifkan fungsi transaksi
<br>2. Sistem menampilkan data member yang sudah mengirimkan data belanja
<br>3. Karyawan memilih data member yang ingin dilihat
<br>4. Sistem menampilkan list belanjaan dari member yang telah dipilih oleh karyawan
<br>5. Jika member memilih membayar secara manual maka kasir menginputkan uang yang dibayarkan oleh member
<br>6. Jika member memilih pembayaran dengan top up maka karyawan langsung melakukan cetak struk dengan menekan tombol cetak struk

__2.2.8 Input data barang Karyawan__

![](http://i66.tinypic.com/ayaj5h.jpg)

Karyawan akan dapat melakukan input barang, dengan cara:
<br>1. Karyawan mengaktifkan fungsi data barang
<br>2. Sistem menampilkan data barang yang sudah ada
<br>3. Karyawan menekan tombol icon tambah
<br>4. Sistem menampilkan form input barang
<br>5. Karyawan mengisi form sesuai dengan requirement
<br>6. Sistem akan melakukan validasi
<br>7. Sistem menyimpan data barang ke dalam database

__2.2.9 Sign Up Toko__

![](http://i64.tinypic.com/16ln1wi.jpg)

Pemilik toko harus mendaftarkan tokonya terlebih dahulu untuk dapat menggunakan aplikasi kami, dengan cara:
<br>1. Pemilik toko mengakses web aplikasi Q-pay
<br>2. Pemilik toko memilih menu daftar toko
<br>3. Sistem menampilkan form pendaftaran toko
<br>4. Pemilik toko mengisi form pendaftaran
<br>5. Pemilik toko menekan tombol daftar
<br>6. Sistem akan melakukan validasi
<br>7. Sistem menyimpan data toko ke dalam database

Kemudian setelah sign up maka pemilik toko diharuskan login, dengan cara :
<br>1. Pemilik toko mengakses web aplikasi Q-pay
<br>2. Pemilik toko memilih menu login
<br>3. Sistem menampilkan form login
<br>4. Pemilik toko mengisi form login
<br>5. Pemilik toko menekan tombol login
<br>6. Sistem akan melakukan validasi dari username dan password
<br>7. Jika username dan password sesuai maka sistem akan menampilkan dashboard pemilik toko
<br>8. Jika username dan password tidak sesuai maka sistem akan meminta pemilik toko untuk mengisi ulang form login

__2.2.10 Lihat laporan penjualan__

![](http://i65.tinypic.com/32zt7at.jpg)

Pemilik toko dapat melihat laporan dari penjualan toko mereka melalui aplikasi kami, dengan cara:
<br>1. Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2. Sistem menampilkan menu untuk pemilik toko
<br>3. Pemilik toko memilih menu laporan penjualan
<br>4. Sistem menampilkan laporan penjualan

__2.2.11 Daftar karyawan__

![](http://i63.tinypic.com/24v4ht4.jpg)

Pemilik toko dapat mendaftarkan atau menambah karyawan toko mereka, dengan cara:
<br>1. Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2. Sistem menampilkan menu untuk pemilik toko
<br>3. Pemilik toko memilih menu tambah karyawan
<br>4. Sistem menampilkan form penambahan karyawan
<br>5. Pemilik toko mengisi form penambahan karayawan
<br>6. Sistem menyimpan data karyawan ke dalam database

__2.2.12 Tarik uang__

![](http://i64.tinypic.com/16ih2j9.jpg)

Pemilik toko dapat mencairkan saldo bagi pembelian produk dengan pembayaran menggunakan e-cash atau top up, dengan cara:

__2.2.13 Input data barang__

![](http://i66.tinypic.com/2jcbhuc.jpg)

Pemilik toko dapat mennambahkan data barang, dengan cara:
<br>1. Pemilik toko masuk ke halaman dashboard pemilik toko
<br>2. Sistem menampilkan menu untuk pemilik toko
<br>3. Pemilik toko memilih menu tambah karyawan
<br>4. Sistem menampilkan form penambahan karyawan
<br>5. Pemilik toko mengisi form penambahan karayawan
<br>6. Sistem menyimpan data karyawan ke dalam database


__2.3 Spesifikasi Kebutuhan Non-Fungsional__
- Availability
<br>Ketersediaan aplikasi yang dapat di-update sewaktu-waktu dan dapat beroperasi terus menerus selama 24 jam per hari tanpa berhenti, karena aplikasi ini akan bersifat android-based dan web-based dan akan diakses oleh pengguna yang membutuhkan dari berbagai tempat pada waktu yang berbeda-beda.
- Security
<br>Aplikasi yang dikembangkan nantinya harus memiliki tingkat keamanan yang tinggi dimana setiap user yang masuk tidak dapat seenaknya mengubah data yang berada di dalam aplikasi ini. Aplikasi ini juga aman karena terdapat transaksi keuangan maka faktor keamanan menjadi sangat penting.
- Usability
<br>Aplikasi ini diharapkan memudahkan user dalam penggunaannya.
- Accessibility
<br>Aplikasi bisa digunakan kapanpun dan dimanapun selama terkoneksi internet.
- Portability
<br>Aplikasi ini memberi kemudahan dalam pengaksesan sistem khususnya terkait dengan faktor waktu dan lokasi pengaksesan, serta perangkat atau teknologi yang digunakan untuk mengakses.

__2.4 Karakteristik pengguna__

__2.5 Batasan-batasan__
- Bahasa pemrograman berbasis android yang digunakan adalah Java.
- Bahasa pemrograman berbasis web yang digunakan adalah PHP dan HTML.
- DBMS yang digunakan adalah MySQL.

__2.6 Asumsi-asumsi keterkaitan__

__2.7 Kebutuhan penyeimbang__
 
##

### BAB III KEBUTUHAN LAIN YANG SPESIFIK

__3.1 Persyaratan Antarmuka Eksternal__
<br>Dalam operasionalnya, aplikasi yang akan dikembangkan memerlukan adanya interaksi dengan komponen-komponen lain diluar perangkat lunak itu seperti, user sebagai seorang pengguna perangkat lunak, perangkat keras dimana perangkat lunak ini akan dijalankan, perangkat komunikasi dimana perangkat lunak ini akan saling berkomunikasi dalam jaringan internet.

__3.2 Functional Requirement__
<p align="justify">
 	Logika Struktur terdapat pada bagian 3.3.1
 </p>

 **3.2.1 Sign In Member dan Karyawan**

| Nama fungsi  |Sign In Member dan Karyawan |
|--|--|
|Ref|Bag 2.1.2, Sign In Member dan Karyawan | 
|Trigger|Membuka aplikasi Q-PAY|
|Precondition|Halaman utama Sign In pada aplikasi|
|Basic Path|1. User mengklik tombol Sign In <br>2. Sistem menampilkan halaman Sign In yang terdiri dari kolom Email dan Password <br>3. User memasukkan Email dan Password <br>4. Sistem mem-validasi Email dan Password|
|Alternative|Tidak Ada|
|Post Condition|User dapat Sign In dan dapat mengakses aplikasi Q-PAY|
|Exception Push	|1. Tidak ada Koneksi <br>2. User belum mendaftar ke aplikasi|

**3.2.2 Lupa Password Member dan Karyawan**

| Nama fungsi  |Lupa Password Member dan Karyawan |
|--|--|
|Ref|Bag 2.1.2, Lupa Password Member dan Karyawan | 
|Trigger|Membuka aplikasi Q-PAY lalu mengklik tombol Lupa Password|
|Precondition|Halaman utama Lupa Password|
|Basic Path|1. User mengklik tombol Lupa Password <br>2. Sistem menampilkan halaman Lupa Password yang berisikan kolom Email yang harus diisikan <br>3. User memasukkan Email <br>4. Sistem mengirim verifikasi melalui Email user|
|Alternative|Tidak Ada|
|Post Condition|User dapat Sign In dan dapat mengakses aplikasi Q-PAY|
|Exception Push	|1. Tidak ada Koneksi <br>2. User belum mendaftar ke aplikasi|

**3.2.3 Sign Up Member**

| Nama fungsi  |Sign Up  |
|--|--|
|Ref|Bag 2.1.2, Sign Up member | 
|Trigger|Membuka aplikasi Q-PAY lalu mengklik tombol Sign Up|
|Precondition|Halaman utama Sign Up pada aplikasi|
|Basic Path|1. Member mengklik tombol Sign Up <br>2. Sistem menampilkan halaman Sign Up yang terdiri dari kolom Nama Lengkap, Alamat, No.Hp, Email dan Password <br>3. Member memasukkan Nama Lengkap, Alamat, No.Hp, Email dan Password <br>4. Sistem menyimpan Nama Lengkap, Alamat, No.Hp, Email dan Password dari member|
|Alternative|Tidak Ada|
|Post Condition|User dapat Sign Up, Login dan dapat mengakses aplikasi Q-PAY|
|Exception Push	|Tidak ada Koneksi|

**3.2.4 Navbar Member**

| Nama fungsi  |Navbar Menu Member  |
|--|--|
|Ref|Bag 2.1.2, Navbar Menu Member | 
|Trigger|Mengklik tombol Navbar Menu|
|Precondition|Halaman utama profile member dan daftar menu aplikasi|
|Basic Path|1. Member mengklik tombol navbar menu <br>2. Sistem menampilkan halaman profile member dan daftar menu yang terdiri dari menu Scan, Daftar Belanja, Top Up, Struk, Setting Profile dan Logout|
|Alternative|Tidak Ada|
|Post Condition|Member dapat mengakses menu dari aplikasi Q-PAY|
|Exception Push	|Tidak ada Koneksi|

**3.2.5 Scan QR Code**

| Nama fungsi  |Scan QR Code |
|--|--|
|Ref|Bag 2.1.2, Scan QR Code | 
|Trigger|Mengklik tombol Scan pada navbar menu|
|Precondition|Halaman utama menu Scan QR Code|
|Basic Path|1. Member mengklik tombol Scan pada navbar menu <br>2. Sistem menampilkan halaman Scan <br>3. Member mengarahkan QR Code scanner pada QR Code bar <br>4. Sistem menampilkan nama dan harga produk|
|Alternative|Tidak Ada|
|Post Condition|Member dapat men-Scan QR Code bar dan mengetahui nama serta harga produk tersebut|
|Exception Push	|Tidak ada Koneksi|

**3.2.6 Daftar Belanja**

| Nama fungsi  |Daftar Belanja |
|--|--|
|Ref|Bag 2.1.2, Daftar Belanja | 
|Trigger|Mengklik tombol Daftar Belanja pada navbar menu|
|Precondition|Halaman utama menu Daftar Belanja|
|Basic Path|1. Member mengklik tombol Daftar Belanja pada navbar menu <br>2. Sistem menampilkan halaman daftar belanja member yang terdiri dari nama barang, qty dan harga|
|Alternative|Tidak Ada|
|Post Condition|Member dapat melihat produk apa saja yang sudah di scan|
|Exception Push	|Tidak ada Koneksi|

**3.2.7 Top Up**

| Nama fungsi  |Top Up |
|--|--|
|Ref|Bag 2.1.2, Top Up | 
|Trigger|Mengklik tombol Top Up pada navbar menu|
|Precondition|Halaman utama menu Top Up|
|Basic Path|1. Member mengklik tombol Top Up pada navbar menu <br>2. Sistem menampilkan halaman top up yang berisikan kolom masukkan kode untuk mengambil saldo dari admin sebagai pembayaran <br>3. Member mengisikan kolom masukkan kode <br>4. Sistem memproses kode|
|Alternative|Tidak Ada|
|Post Condition|Member dapat memasukkan kode untuk memulai proses pengiriman saldo|
|Exception Push	|Tidak ada Koneksi|

**3.2.8 Isi Saldo**

| Nama fungsi  |Isi Saldo |
|--|--|
|Ref|Bag 2.1.2, Isi Saldo | 
|Trigger|Mengklik tombol Isi Saldo pada menu Top Up|
|Precondition|Halaman utama menu Isi Saldo|
|Basic Path|1. Member mengklik tombol Isi Saldo pada menu Top Up <br>2. Sistem menampilkan halaman Isi Saldo yang berisikan daftar pilihan saldo yang dapat member pilih untuk dikirimkan <br>3. Sistem memproses jumlah saldo|
|Alternative|Tidak Ada|
|Post Condition|Member dapat memilih jumlah saldo yang akan dikirimkan|
|Exception Push	|Tidak ada Koneksi|

**3.2.9 Info Transfer**

| Nama fungsi  |Info Transfer |
|--|--|
|Ref|Bag 2.1.2, Info Transfer | 
|Trigger|Mengklik tombol kirim pada menu Isi saldo|
|Precondition|Halaman utama menu Info Transfer|
|Basic Path|1. Member mengklik tombol kirim pada menu Top Up <br>2. Sistem menampilkan halaman Info Transfer yang berisikan kolom no. rekening yang harus diisikan member <br>3. Sistem memproses saldo|
|Alternative|Tidak Ada|
|Post Condition|Member dapat memasukkan no. rekening yang akan dituju untuk pengiriman saldo|
|Exception Push	|Tidak ada Koneksi|


**3.2.10 Struk**

| Nama fungsi  |Struk |
|--|--|
|Ref|Bag 2.1.2, Struk | 
|Trigger|Mengklik tombol Struk pada navbar menu|
|Precondition|Halaman utama menu Struk|
|Basic Path|1. Member mengklik tombol Struk pada navbar menu <br>2. Sistem menampilkan halaman struk yang berisikan struk dari list transaksi|
|Alternative|Tidak Ada|
|Post Condition|Member dapat melihat list transaksi yang pernah dilakukan member di toko tersebut beserta dengan tanggal transaksinya|
|Exception Push	|Tidak ada Koneksi|

**3.2.11 Detail Struk**

| Nama fungsi  |Detail Struk |
|--|--|
|Ref|Bag 2.1.2, Detail Struk | 
|Trigger|Mengklik salah satu dari list pada menu Struk|
|Precondition|Halaman utama menu Detail Struk|
|Basic Path|1. Member mengklik salah satu dari list pada menu struk <br>2. Sistem menampilkan halaman detail struk yang berisikan nama barang, qty dan harga produk|
|Alternative|Tidak Ada|
|Post Condition|Member dapat melihat struk secara detail|
|Exception Push	|Tidak ada Koneksi|

**3.2.12 Setting Profile Member**

| Nama fungsi  |Setting Profile Member|
|--|--|
|Ref|Bag 2.1.2, Setting Profile Member| 
|Trigger|Mengklik tombol Setting Profile pada navbar menu|
|Precondition|Halaman utama menu Setting Profile|
|Basic Path|1. Member mengklik tombol Setting Profile pada navbar menu <br>2. Sistem menampilkan halaman Setting Profile yang berisikan kolom data diri member <br>3. Member mengklik salah satu kolom data diri dan mengubah isi dari data pada kolom tersebut <br>4. Sistem memproses dan menyimpan data tersebut|
|Alternative|Tidak Ada|
|Post Condition|Member dapat mengubah data dirinya|
|Exception Push	|Tidak ada Koneksi|

**3.2.13 Setting Foto Profile Member**

| Nama fungsi  |Setting Foto Profile Member|
|--|--|
|Ref|Bag 2.1.2, Setting Foto Profile Member| 
|Trigger|Mengklik foto profile pada menu setting profile|
|Precondition|Halaman utama menu Setting Foto Profile|
|Basic Path|1. Member mengklik foto profile pada menu setting profile <br>2. Sistem menampilkan halaman Setting Foto Profile yang berisikan pilihan pengambilan foto <br>3. Sistem memproses dan menyimpan foto profile tersebut|
|Alternative|Tidak Ada|
|Post Condition|Member dapat mengubah foto profilenya|
|Exception Push	|Tidak ada Koneksi|

**3.2.14 Navbar Karyawan**

| Nama fungsi  |Navbar Menu Karyawan|
|--|--|
|Ref|Bag 2.1.2, Navbar Menu Karyawan| 
|Trigger|Mengklik tombol Navbar Menu|
|Precondition|Halaman utama profile karyawan dan daftar menu aplikasi|
|Basic Path|1. Karyawan mengklik tombol navbar menu <br>2. Sistem menampilkan halaman profile member dan daftar menu yang terdiri dari menu Data Barang, Transaksi, Setting Profile dan Logout|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat mengakses menu dari aplikasi Q-PAY|
|Exception Push	|Tidak ada Koneksi|

**3.2.15 Transaksi Penjualan**

| Nama fungsi  |Transaksi Penjualan|
|--|--|
|Ref|Bag 2.1.2, Transaksi Penjualan| 
|Trigger|Mengklik tombol Transaksi Penjualan pada menu pilihan Transaksi|
|Precondition|Halaman utama Transaksi Penjualan|
|Basic Path|1. Karyawan mengklik tombol transaksi lalu mengklik salah satu pilihan Transaksi Penjualan <br>2. Sistem menampilkan halaman Transaksi Penjualan yang berisikan list transaksi antara toko dengan member|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat melihat list dari transaksi penjualan|
|Exception Push	|Tidak ada Koneksi|

**3.2.16 Transaksi Pembelian**

| Nama fungsi  |Transaksi Pembelian|
|--|--|
|Ref|Bag 2.1.2, Transaksi Pembelian| 
|Trigger|Mengklik tombol Transaksi Pembelian pada menu pilihan Transaksi|
|Precondition|Halaman utama Transaksi Pembelian|
|Basic Path|1. Karyawan mengklik tombol transaksi lalu mengklik salah satu pilihan Transaksi Pembelian <br>2. Sistem menampilkan halaman Transaksi Pembelian yang berisikan list transaksi antara toko dengan pemasok yang melakukan supplay barang|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat melihat list dari transaksi penjualan|
|Exception Push	|Tidak ada Koneksi|

**3.2.17 Detail Transaksi**

| Nama fungsi  |Detail Transaksi|
|--|--|
|Ref|Bag 2.1.2, Detail Transaksi| 
|Trigger|Mengklik salah satu dari list pada menu Transaksi|
|Precondition|Halaman utama menu Detail Transaksi|
|Basic Path|1. Karyawan mengklik salah satu dari list pada menu transaksi <br>2. Sistem menampilkan halaman detail transaksi yang berisikan nama barang, qty dan harga produk|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat melihat transaksi secara detail|
|Exception Push	|Tidak ada Koneksi|

**3.2.17 Input Bayar**

| Nama fungsi  |Input Bayar|
|--|--|
|Ref|Bag 2.1.2, Input Bayar| 
|Trigger|Mengklik tombol cetak pada menu Detail Transaksi|
|Precondition|Halaman utama menu Input Bayar|
|Basic Path|1. Karyawan mengklik tombol cetak pada menu Detail Transaksi <br>2. Sistem menampilkan halaman input bayar <br>3. Karyawan memasukkan jumlah yang akan dibayarkan <br>4. Sistem memproses pembayaran|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat melakukan pembayaran dengan memasukkan jumlah bayar|
|Exception Push	|Tidak ada Koneksi|

**3.2.18 Input Data Barang**

| Nama fungsi  |Input Data Barang|
|--|--|
|Ref|Bag 2.1.2, Input Data Barang| 
|Trigger|Mengklik tombol Data Barang pada menu navbar|
|Precondition|Halaman utama menu Input Data Barang|
|Basic Path|1. Karyawan mengklik tombol Input Data Barang pada menu navbar <br>2. Sistem menampilkan halaman Input Data Barang yang berisikan kolom Nama Barang, Harga Beli, Harga Jual, Satuan dan Stok <br>3. Karyawan memasukkan isi dari tiap kolom Input Data Barang <br>4. Sistem memproses dan menyimpan data barang|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat melakukan pembayaran dengan memasukkan jumlah bayar|
|Exception Push	|Tidak ada Koneksi|

**3.2.19 Setting Profile Karyawan**

| Nama fungsi  |Setting Profile Karyawan|
|--|--|
|Ref|Bag 2.1.2, Setting Profile Karyawan| 
|Trigger|Mengklik tombol Setting Profile pada navbar menu|
|Precondition|Halaman utama menu Setting Profile|
|Basic Path|1. Karyawan mengklik tombol Setting Profile pada navbar menu <br>2. Sistem menampilkan halaman Setting Profile yang berisikan kolom data diri karyawan <br>3. Karyawan mengklik salah satu kolom data diri dan mengubah isi dari data pada kolom tersebut <br>4. Sistem memproses dan menyimpan data tersebut|
|Alternative|Tidak Ada|
|Post Condition|Member dapat mengubah data dirinya|
|Exception Push	|Tidak ada Koneksi|

**3.2.20 Setting Foto Profile Karyawan**

| Nama fungsi  |Setting Foto Profile Karyawan|
|--|--|
|Ref|Bag 2.1.2, Setting Foto Profile Karyawan| 
|Trigger|Mengklik foto profile pada menu setting profile|
|Precondition|Halaman utama menu Setting Foto Profile|
|Basic Path|1. Karyawan mengklik foto profile pada menu setting profile <br>2. Sistem menampilkan halaman Setting Foto Profile yang berisikan pilihan pengambilan foto <br>3. Sistem memproses dan menyimpan foto profile tersebut|
|Alternative|Tidak Ada|
|Post Condition|Karyawan dapat mengubah foto profilenya|
|Exception Push	|Tidak ada Koneksi|

__3.3 Struktur Detail Kebutuhan Non-Fungsional__

____3.3.1 Logika Struktur Data____
<br>Struktur data logika pada aplikasi ini terdapat struktur Database yang dijelaskan menggunakan ERD berikut :<br>

![](http://i68.tinypic.com/msknkw.jpg)

Deskripsi dapat dijelaskan seperti berikut:<br>

<b>Tabel User</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_user |Integer|id user auto increment|
|email|Varchar|email yang digunakan user untuk login|
|password|Varchar|password yang digunakan user untuk login|
|level|Varchar|level user untuk login seperti member, karyawan, admin, dan pemilik toko|

<b>Tabel Member</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_member|Integer|Id member auto increment|
|id_user|Integer|Relasi untuk menghubungkan akun user dengan data member|
|nama|Varchar|Nama member|
|email|Varchar|Email member|
|alamat|Varchar|Alamat member|
|no_hp|Varchar|Nomor hp member|
|jumlah_saldo|Integer|Jumlah saldo member|

<b>Tabel Toko</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_toko|Integer|Id toko auto increment|
|id_user|Integer|Relasi untuk menghubungkan akun user dengan data toko|
|nama_toko|Varchar|Nama toko|
|nama_pemilik_toko|Varchar|Nama pemilik toko|
|alamat_toko|Varchar|Alamat toko|
|email|Varchar|Email pemilik toko atau email toko|
|jumlah_saldo|Integer|Jumlah saldo toko|

<b>Tabel Karyawan</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_karyawan|Integer|Id karyawan auto increment|
|id_user|Integer|Relasi untuk menghubungkan akun user dengan data karyawan|
|id_toko|Integer|Relasi untuk menghubungkan data karyawan dengan data toko|
|nama|Varchar|Nama karyawan|
|email|Varchar|Email karyawan|
|no_hp|Varchar|Nomor hp karyawan|
|alamat|Varchar|Alamat karyawan|

<b>Tabel Pemasok</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_pemasok|Integer|Id pemasok auto increment|
|id_toko|Integer|Relasi untuk menghubungkan data pemasok dengan data toko|
|nama|Varchar|Nama pemasok|
|no_hp|Varchar|Nomor hp pemasok|
|alamat|Varchar|Alamat pemasok|

<b>Tabel Barang</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_barang|Integer|Id barang auto increment|
|id_toko|Integer|Relasi untuk menghubungkan data barang dengan data toko|
|nama_barang|Varchar|Nama barang|
|harga_beli|Integer|Harga beli barang|
|harga_jual|Integer|Harga jual barang|
|satuan|Varchar|Satuan dari barang|
|stok|Integer|Stok barang yang tersedia di toko|

<b>Tabel Transaksi_Penjualan</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_jual|Integer|Id transaksi penjualan auto increment|
|id_toko|Integer|Relasi untuk menghubungkan data transaksi penjualan dengan data toko|
|id_member|Integer|Relasi untuk menghubungkan data transaksi penjualan dengan data member|
|id_karyawan|Integer|Relasi untuk menghubungkan data transaksi penjualan dengan data karyawan|
|tanggal|date|Tanggal transaksi penjualan dilakukan|
|total_harga|Integer|Total harga dari transaksi penjualan|
|cara_pembayaran|Varchar|Cara pembayaran member saat transaksi penjualan|

<b>Tabel Detail_Transaksi_Penjualan</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_detail_jual|Integer|Id detail transaksi penjualan auto increment|
|id_jual|Integer|Relasi untuk menghubungkan data detail transaksi penjualan dengan data transaksi penjualan|
|id_barang|Integer|Relasi untuk menghubungkan data detail transaksi penjualan dengan data barang|
|quantity|Integer|Quantity dari barang yang di jual|
|harga|Integer|Harga barang setelah dikali dengan quantity|

<b>Tabel Transaksi_Pembelian</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_beli|Integer|Id transaksi pembelian auto increment|
|id_toko|Integer|Relasi untuk menghubungkan data transaksi pembelian dengan data toko|
|id_pemasok|Integer|Relasi untuk menghubungkan data transaksi pembelian dengan data pemasok|
|id_karyawan|Integer|Relasi untuk menghubungkan data transaksi pembelian dengan data karyawan|
|tanggal|Date|Tanggal transaksi pembelian dilakukan|
|total_harga|Integer|Total harga dari transaksi pembelian|

<b>Tabel Detail_Transaksi_Pembelian</b>

|Data Item| Type | Deskripsi|
|--|--|--|
|id_detail_beli|Integer|Id detail transaksi pembelian auto increment|
|id_beli|Integer|Relasi untuk menghubungkan data detail transaksi pembelian dengan data transaksi pembelian|
|id_barang|Integer|Relasi untuk menghubungkan data detail transaksi pembelian dengan data barang|
|quantity|Integer|Quantity dari barang yang di beli|
|harga|Integer|Harga barang setelah dikali dengan quantity|
