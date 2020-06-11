#Kubernetes 
Kubernetes merupakan platform open-source yang digunakan untuk melakukan manajemen workloads aplikasi yang dikontainerisasi, serta menyediakan konfigurasi dan otomatisasi secara deklaratif. Kubernetes berada di dalam ekosistem yang besar dan berkembang cepat. Service, support, dan perkakas Kubernetes tersedia secara meluas.
Google membuka Kubernetes sebagai proyek open source pada tahun 2014. Kubernetes dibangun berdasarkan pengalaman Google selama satu setengah dekade dalam menjalankan workloads bersamaan dengan kontribusi berupa ide-ide terbaik yang diberikan oleh komunitas.

Kubernetes memiliki sejumlah fitur yang dapat dijabarkan sebagai berikut:
platform kontainer
platform microservices
platform cloud yang tidak mudah dipindahkan
Kubernetes menyediakan manajemen environment yang berpusat pada kontainer. Kubernetes melakukan orkestrasi terhadap computing, 
networking, dan inftrastruktur penyimpanan. Fitur inilah yang kemudian membuat konsep Platform as a Service (PaaS) menjadi lebih
sederhana dilengkapi dengan fleksibilitas yang dimiliki oleh Infrastructure as a Service (IaaS.
Meskipun Kubernetes menyediakan banyak fungsionalitas, selalu ada keadaan dimana hal tersebut membutuhkan fitur baru. Workflow spesifik yang terkait dengan proses pengembangan aplikasi dapat ditambahkan pada streamline untuk meningkatkan produktivitas developer. Orkestrasi ad-hoc yang dapat diterima biasanya membutuhkan desain otomatisasi yang kokoh agar bersifat scalable. Hal inilah yang membuat Kubernetes juga didesain sebagai platform untuk membangun ekosistem komponen dan dan perkakas untuk memudahkan proses deployment, scale, dan juga manajemen aplikasi.

Labels memudahkan pengguna mengkategorisasikan resources yang mereka miliki sesuai dengan kebutuhan. Annotations memungkinkan pengguna untuk menambahkan informasi tambahan pada resource yang dimiliki.
Selain itu, Kubernetes control plane dibuat berdasarkan API yang tersedia bagi pengguna dan developer. Pengguna dapat mengimplementasikan kontroler sesuai dengan kebutuhan mereka, contohnya adalah schedulers, dengan API kustom yang mereka miliki, kontroler kustom ini kemudian dapat digunakan pada command-line tool generik yang ada.
Desain inilah yang memungkinkan beberapa sistem lain untuk dapat dibangun di atas Kubernetes.
