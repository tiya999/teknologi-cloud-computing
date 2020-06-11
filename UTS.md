
Pertemuan 5
Pengertian Business Process as a Service
Proses Bisnis sebagai Layanan (BPaaS) adalah setiap jenis proses bisnis horizontal atau vertikal yang disampaikan berdasarkan model layanan awan. Layanan awan ini - yang meliputi Software sebagai Service (SaaS), Platform sebagai Layanan (PaaS), dan Infrastructure as a Service (IaaS) - karena itu tergantung pada layanan terkait. 
Perusahaan telah mengotomatisasi proses bisnis selama beberapa dekade. Awalnya, mereka dipaksa untuk melakukannya secara manual atau pemrograman. Sebagai contoh, jika sebuah perusahaan ingin memastikan bahwa sistem manajemen untuk pesanan mendongak pemeriksaan kredit sebelum mengeluarkan transaksi, perusahaan membangun bahwa permintaan ke dalam program. 
Dalam beberapa kasus, seluruh proses bisnis outsourcing perusahaan mungkin menerapkan proses secara manual atau melalui otomatisasi. Dengan munculnya komputasi awan, pendekatan ini mulai berubah. Semakin, perusahaan sedang melihat pendekatan berorientasi-layanan yang lebih kepada pelayanan. Daripada berasumsi bahwa Anda perlu paket aplikasi yang meliputi logika bisnis, data, dan proses, itu mungkin untuk memilih aplikasi proses yang tidak terikat ke satu aplikasi.
Latihan
Cara mengistal Apache OFBiz
Apache OFBiz adalah suatu framework+common data model+ business process atau aplikasi ERP dan dibangun dengan Pemrogaman Java. Semua aplikasi dibuat dengan menggunakan arsitektur yang umum, menggunakan komponen-komponen data, logic dan process.
Apache OFBiz menawarkan fleksibilitas desain dan akses terhadap kode program sehingga memudahkan melakukan modifikasi. Saat ini fungsionalitas yang tersedia pada OFBiz adalah E-Commerce, Manajemen Katalog, Manajemen Promosi dan Pricing, Manajemen Order, Manajemen Customer, Manajemen Pergudangan, Persediaan, Akuntansi, Manajemen Produksi, Manajemen Konten.

Berikut adalah tutorial cara menginstall Apache Ofbiz.tools yang perlu dipersiapkan untuk menginstall Apache Ofbiz adalah :
Apache Ofbiz
Gradle atau Apache ant
JDK ( Java Development Kit)
JDK merupakan software yang digunakan untuk melakukan proses kompilasi dari java code ke bytecode yang dapat dimengerti dan dapat dijalankan oleh JRE (Java Runtime Envirotment).
1.	Sebelum menginstall Apache ofbiz pastikan laptop/pc anda sudah terinstal Java terlebih dahulu,untuk mengetahui apakah java sudah terinstall atau belum silakan ketik java dan javac di command prompt.
2.	setelah java terinstall selanjutnya ekstrak file grandel dan apache ofbiz yang telah di download tadi.
lalu copykan folder kedua file yang telah anda ekstrak tadi ke path yang ada di system variabel .kemudian  kedua folder tadi tercopy ke path yang ada di system variabel selanjutnya kita akan menginstall Apache ofbiz melalui Command prompt.
3.	Buka command prompt cari folder apache ofbiz yang sudah diekstrak tadi seperti 
4.	kemudian install gradle atau apache ant untuk mengkompilasi source code menjadi executable  
5.	Ketikkan ant load-demo untuk mengisikan data ke database demo, maka hasilnya seperti di bawah ini dan tunggu proses installasn selesai


6.	Setelah proses selesai maka jalankan Apache ofbiz dengan perintah ant start
7.	Apache ofbiz telah selesai diinstall. Sekarang kita coba menjalankan Apache ofbiz yang telah selesai diinstall tadi dengan mengetikkan https://127.0.0.1:8443/catalog/control/main di web browser.
8.	masukkan username dan password,setelah username dan password dimasukkan 
Apache ofbiz telah selesai di install dan bisa digunakan.
