Cara Instal MongoDB Pada OS Windows
Dalam postingan ini saya menggunakan sistem operasi windows 10 64 bit untuk menginstall mongoDB versi 2.6.4. anda bisa mendapatkan file installer untuk sistem operasi widnwos pada webiste resmi mongodb.com. setelah selesai proses download silahkan double click pada file installer dan ikuti proses instalasi sebagai berikut :
1.	 klik Install untuk melanjutkan proses install MongoDB pada OS Windows
2.	Pilih custom untuk menentukan lokasi installasi mongoDB secara manual
3.	Pilih partisi C atau partisi lain yang akan menjadi lokasi kita melakukan instalasi MongoDB pada sistem operasi windows, selanjutnya buatlah sebuah folder baru dengan nama mongodb dan pilihlah folder ini sebagai tujuan instalasi seperti gamabr diatas, kemudian klik OK untuk melanjutkan instalasi mongoDB
4.	Tunggu sejenak sampai proses instalasi mongoDB selesai, biasanya membutuhkan waktu sekitar 3 menit.
5.	Klik finish untuk mengakhiri proses instalasi MongoDB, sampai pada tahap ini anda sudah berhasil melakukan proses instalasi mongoDB pada OS Windows.
Menjalankan Server Mogodb
Setelah tahap instalasi selesai maka kita akan mencoba menggunakan nya, langkah yang pertama harus anda lakukan adalah buka CMD kemudian masuk ke lokasi/ path mongoDB yang ada pad direktori C:\mongodb\bin dan mengaktifkan server mongoDB dengan cara :
mongod.exe --dbpath=c:\mongodb\data
jika berhasil maka akan muncul pesan waiting for connection 

Membuat Service MongoDB
pertanyaan selanjutnya adalah apakah anda harus melakukan perintah menjalankan mongoDB secara manual setiap ingin digunakan ? tentunya tidak, kita bisa membuat sebuah service yang membantu kita dalam mengelola proses dari mongoDB itu sendiri, dan kita bisa mengatur service yang sudah dibuat agar dijalankan otomatis ketika komputer di gunakan melalui service manager. cara membuat service mongodb adalah sebagai berikut :
mongod.exe –install –journal –logpath c:\mongodb\ mongo.log –dbpath=c:\mongodb\data
	
lalu silahkan restart komputer/ PC anda setelah proses pembuatan service berhasil.
Management Service MongoDB Pada OS Windows
seperti layaknya service pada sistem operasi windows, kita juga bisa melakukan management service MogonDB baik melalui CMD ataupun Service Manager Windows. berikut ini adalah cara melakukan management service MongoDB melalui CMD pada sistem operasi Windows.
Merunning/ mengaktifkan service mongoDB
net start mongodb
Mengstop/ menghentikan service MongoDB
net stop mongodb
Merestart service MongoDB
C:\monogdb\mongod.exe --remove
sampai pada tahap ini anda sudah berhasil menginstall MongoDB pada sistem operasi windows, pada artikel selanjutnya kita akan belajar cara melakukan management database menggunakan MongoDB.



