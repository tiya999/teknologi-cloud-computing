Docker : Assign to Containers
Langsung saja.
Pertama, lihat dulu base image nya :
# docker images
Lalu bisa dilihat tabel base network nya secara default :
# docker network ls
Nah, sebelum me-assign network kedalam container, kita buat dulu networknya, misal :
# docker network create --subnet 10.0.0.0/16 --gateway 10.0.0.1 --ip-range=10.0.3.0/24 --driver=bridge --label=hostnetwork3 bridge03
Keterangan :
create –subnet 10.0.0.0/16 = Membuat subnetwork 10.0.0.0/16
–gateway 10.0.0.1 = gateway yang digunakan adalah 10.0.0.1
–ip-range=10.0.3.0/24 = Range IP Address untuk host client
–driver=bridge = Driver untuk network
–label=hostnetwork3 = label
bridge03 = Nama untuk network
Bisa cek juga dengan :
# ifconfig
Lalu lihat base network kembali :
# docker network ls
Bisa dilihat pula menggunakan perintah berikut untuk melihat detail network bridge03 :
# docker inspect bridge03
Selanjutnya, setelah membuat network kita bisa membuat container baru dengan menggunakan network yang tadi :
# docker run -it --name networktest1 --net bridge03 centos:latest /bin/bash
Selanjutnya, bisa diupdate dan install net-tools untuk melihat ip address nya apakah sudah sesuai atau belum :
# yum -y update
# yum -y install net-tools
Lalu jalankan :
# ifconfig
Sesuai.
Untuk selanjutnya, kita akan mencoba membuat container baru dimana IP Address sudah ditetapkan langsung saat container pertamakali berjalan. Ini istilahnya seperti reservasi IP Address.
Bisa jalankan perintah :
# docker run -it --name networktest2 --net bridge03 --ip 10.0.3.123 centos:latest /bin/bash
Coba update dan install net-tools lagi untuk mengecek IP Address dari container :
# yum -y update && yum -y install net-tools
Lalu cek IP Address :
# ifconfig
Atau bisa dengan membuka tab baru, pastikan container masih aktif :
# docker ps
Dan jalankan command inspect :
# docker inspect networktest2 | grep IPAdd
