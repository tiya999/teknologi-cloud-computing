DevStack
 adalah serangkaian skrip yang dapat diperluas yang digunakan untuk dengan cepat memunculkan lingkungan OpenStack lengkap berdasarkan versi terbaru dari segalanya dari git master. Ini digunakan secara interaktif sebagai lingkungan pengembangan dan sebagai dasar untuk banyak pengujian fungsional proyek OpenStack. Sumber tersedia di https://opendev.org/openstack/devstack.
Langka -langka
Instal Linux
Mulailah dengan instalasi sistem Linux yang bersih dan minimal. DevStack berupaya mendukung dua rilis LTS terbaru Ubuntu, versi Fedora terbaru / saat ini, CentOS / RHEL 7, serta Debian dan OpenSUSE.

Jika Anda tidak memiliki preferensi, Ubuntu 18.04 (Bionic Beaver) adalah yang paling diuji, dan mungkin akan menjadi yang paling lancar.

Tambahkan Stack User (opsional) 
DevStack harus dijalankan sebagai pengguna non-root dengan sudo diaktifkan (login standar ke gambar cloud seperti "ubuntu" atau "pengguna cloud" biasanya baik-baik saja).

Jika Anda tidak menggunakan gambar cloud, Anda dapat membuat pengguna tumpukan terpisah untuk menjalankan DevStack
$ sudo useradd -s /bin/bash -d /opt/stack -m stack
Karena pengguna ini akan membuat banyak perubahan pada sistem Anda, ia harus memiliki hak sudo:
$ echo "stack ALL=(ALL) NOPASSWD: ALL" | sudo tee /etc/sudoers.d/stack
$ sudo su - stack

Download DevStack
$ git clone https://opendev.org/openstack/devstack
$ cd devstack
Repo devstack berisi skrip yang menginstal OpenStack dan templat untuk file konfigurasi.
Create a local.conf¶
Create a local.conf dengan empat kata sandi yang telah ditetapkan pada akar repo devstack git.
[[local|localrc]]
ADMIN_PASSWORD=secret
DATABASE_PASSWORD=$ADMIN_PASSWORD
RABBIT_PASSWORD=$ADMIN_PASSWORD
SERVICE_PASSWORD=$ADMIN_PASSWORD

Mulai instal
$ ./stack.sh

Ini akan memakan waktu 15 - 20 menit, sebagian besar tergantung pada kecepatan koneksi internet Anda. Banyak pohon dan paket git akan diinstal selama proses ini.


