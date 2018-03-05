<html>
<body>
<p align="center"><h1> Software Requirements Spesification </h1></p>

<p align="center"><b>Version 1.0.4 </b><br>
<p align="center">12 Februari 2018</b><br><br>
<p align="center">
<img src="https://2.bp.blogspot.com/-dxdRgMQGbLk/WpA-Tp2rNGI/AAAAAAAAAh8/3_jBWFb7Cf48033QvB34D2WCwoN2sxZLgCLcBGAs/s1000/index.png"/>
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
<p align="center"><b>2018</b><br><br>
</p>
</body>
</html>

##
##
## 1. BAB I Pendahuluan
<br>Dokumen ini berisi penjelasan pemakaian dan penulisan dokumen Spesifikasi Kebutuhan Perangkat Lunak (SKPL) atau Software Requirement Specification (SRS). Dokumen ini selanjutnya akan menggunakan istilah SRS.

Software Requirement Specification (SRS) menjelaskan berbagai macam kebutuhan pembuatan produk, yaitu kebutuhan spesifik yang terdiri dari kebutuhan fungsionalitas, termasukdidalamnya input, proses, dan output dari produk dan non-fungsionalitas. Kebutuhan antar muka juga digambarkan dengan jelas di dalam dokumen ini, terdiri dari kebutuhan antar pengguna, antar hardware yang menjelaskan kebutuhan yang harus ada untuk menjalankan atau mengoperasikan aplikasi sistem, kebutuhan antar software yang menjelaskan bagaimana cara pengguna berinteraksi dengan sistem, dan kebutuhan antar komunikasi.

Dokumen ini dibuat untuk membantu membuat spesifikasi perangkat lunak yang akan dikembangkan dengan rancangan berorientasi proses. Pada prinsipnya, hasil analisis sistem perangkat lunak dengan rancangan ini diuraikan sebagai sekumpulan proses yang terorganisasi secara hirarkis, memberikan solusi, batasan masalah agar proyek tidak menyimpang terlalu jauh dari tujuan awal, dan manfaat dari sistem informasi yang akan dibuat. Software Requirement Spesification ini dapat dijadikan acuan agar proyek dapat berjalan dengan lancar selama pengerjaannya.

__1.1 Tujuan__
<br>Tujuan dari dokumen Software Requirement Specification (SRS) ini adalah memberikan gambaran yang spesifik dari kebutuhan software. Spesifikasi kebutuhan tersebut termasuk dari segi perangkat lunak dan perangkat keras, untuk memberikan gambaran dan penjelasan mengenai pembuatan produk, penjelasan hal-hal yang dibutuhkan untuk pembuatan produk termasuk kebutuhan fungsional hingga nonfungsional, dan kebutuhan antar muka mulai dari antar muka pengguna hingga antar muka komunikasi.

__1.2 Lingkup__
<br>Semua hal yang tercantum didalam dokumen ini merupakan bagian dari ruang lingkup kebutuhan pembangunan perangkat lunak yang berupa aplikasi kasir QR Code berbasis android yang digunakan untuk perhitugan keuangan pada toko-toko.

__1.3 Definitions, Acronyms and Abbreviations__
<br>a. SRS/SKPL adalah dokumen yang menggambarkan secara detail spesifikasi kebutuhan software dalam pembangunan proyek perangkat lunak Aplikasi Kasir QR Code Berbasis Android.
b. DFD adalah suatu diagram yang menggunakan notasi-notasi untuk menggambarkan arus dari data pada suatu sistem atau menjelaskan proses kerja suatu sistem, yang penggunaannya sangat membantu untuk memahami sistem secara logika, tersruktur dan jelas.
c. Software : Perangkat Lunak.
d. Hardware : Perangkat Keras
e. SRS : Software Requirements Specification.
f. SKPL : Spesifikasi Kebutuhan Perangkat Lunak
g. DFD : Data Flow Diagram
h. IEEE : The Institute of Electrical and Electronics Engineers

__1.4 References__
<br>IEEE Std. 830-1998, IEEE Recommended Practice for Software Requirement Specifications.

__1.5 Overview__
<br>Dokumen SRS ini merupakan acuan untuk mengetahui spesifikasi kebutuhan dalam menyelesaikan proyek ini. Dokumen SRS ini berisi tentang deskripsi tentang kebutuhan perangkat lunak (tools pendukung, peranangan sistem yang akan dikembangkan), perangkat keras, dan sumber daya manusia (SDM)

## BAB II GAMBARAN UMUM
<br>Pada umumnya toko-toko yang tidak terlalu besar metode transaksi pembayarannya manual seperti ditulis dikertas lalu di jumlah dengan kalkulator, dengan metode seperti itu memakan waktu dan tidak efisien, karena untuk transaksi pembayaran harus cepat dan tepat patal jadinya jika penghitungan salah, toko dapat merugi, ditambah pohon-pohon yang ada di muka semakin menipis, ini terjadi karena pohon menjadi bahan baku pembuatan kertas, semakin sedikitnya pohon, bumi semakin panas dan cuaca pun tidak menentu, dan sudah jelas kerusakan alam sudah mulai terlihat akibat pohon-pohon dimuka bumi ini berkurang.

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

<br>Dalam penggunaan & pengguna berinteraksi langsung dengan aplikasi melalui android.

![use case 1](http://i68.tinypic.com/263vbrs.jpg)

____2.1.2 Antarmuka pengguna____

![phone](http://i66.tinypic.com/30cyg7q.png)
![opening app](http://i65.tinypic.com/k48ms7.png)
![sign in user](http://i64.tinypic.com/rr73uh.png)
![sign up user](http://i64.tinypic.com/554ax0.png)
![home user](http://i63.tinypic.com/2u6k4js.png)
![home menu user](http://i65.tinypic.com/20itelf.png)
![scan menu](http://i68.tinypic.com/eb6649.png)
![scan pop up](http://i63.tinypic.com/m75qom.png)
![scan berhasil](http://i67.tinypic.com/2aeyud1.png)
![top up](http://i65.tinypic.com/6j28w5.png)
![bayar dgn top up](http://i66.tinypic.com/28k6hc3.png)
![struk](http://i68.tinypic.com/2hx7tr9.png)
![struk det](http://i64.tinypic.com/334p8ie.png)
![login kary](http://i65.tinypic.com/szfx53.png)
![menu kary](http://i67.tinypic.com/34j3fyc.png)
![home menu kary](http://i64.tinypic.com/xlbk06.png)
![data brg](http://i68.tinypic.com/wcl84j.png)

____2.1.3 Antarmuka perangkat keras____
<br>Kebutuhan minimum perangkat keras yang dapat digunakan oleh aplikasi ini adalah :
- Android

____2.1.4 Antarmuka perangkat lunak____
<br>Perangkat lunak yang dibutuhkan untuk aplikasi ini yaitu :
<ul>
<li>Android Studio</li>
<li>Sublime Teks</li>
<li>XAMPP</li>
<li>Balsamiq Mockup3</li>
</ul>

____2.1.5 Antarmuka komunikasi____
<br>Yang dibutuhkan hanya sebuah android yang dapat terhubung ke internet.

____2.1.6 Batasan-batasan memori____
<br>Perangkat lunak hanya dapat dijalankan di android.

____2.1.7 Operasi-operasi____

____2.1.8 Kebutuhan-kebutuhan dalam tahapan adaptasi____

__2.2 Fungsi-fungsi produk__

![use case 2](http://i68.tinypic.com/2cnjx9f.jpg)

__2.3 Karakteristik pengguna__

__2.4 Batasan-batasan__

__2.5 Asumsi-asumsi dan ketergantungan/keterkaitan__


## BAB III KEBUTUHAN LAIN YANG SPESIFIK
<br>Kebutuhan fungsional adalah kebutuhan yang harus dipenuhi agar suatu sistem dapat berjalan atau dapat dikatakan kebutuhan tambahan yang memiliki input, proses dan output. Kebutuhan fungsional yang harus ada dalam sistem yang akan dikembangkan ini yaitu sistem harus dapat mempermudah pengguna dalam menggunkan aplikasi ini.


## BAB IV INFORMASI PENDUKUNG
