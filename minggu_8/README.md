Langkah Mengelola Docker Container
Mengetahui container apa saja yang sudah kamu jalankan gunakan command :
- docker ps
Melihat seluruh container yang sudah kamu buat baik yang aktif maupun tidak aktif jalankan command :
- docker ps -a
menjalankan dan menghentikan container kamu bisa menggunakan command docker start / stop lalu diikuti dengan nama atau id dari container tersebut.
Menjalankan :
- docker start agitated_tu
Menghentikan :
- docker stop agitated_tu
menghapus container gunakan command berikut :
- docker rm agitated_tu

Langkah Commit Perubahan ke Docker Image
Jika kamu pernah bekerja dengan sebuah version control seperti git, maka dengan docker kamu akan menemui hal yang cukup mirip.
Kamu dapat membuat sebuah image baru dengan beberapa perubahaan.
Secara sederhana, command untuk melakukan hal tersebut adalah sebagai berikut :
- docker commit -m "Catatan tentang apa yang kamu lakukan" -a "Nama pembuat" container-id repository/new_image_name
Contoh :
- docker commit -m "Tambah nodejs sob!" -a "jagoanhostingkece" a8b5756c57d2 jagoanhostingkece/ubuntu-nodejs
Cek image kamu dengan command :
- docker images
