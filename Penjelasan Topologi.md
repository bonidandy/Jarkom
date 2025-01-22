Penjelasan Topologi Jaringan  

Topologi jaringan dalam gambar menunjukkan koneksi antara tiga kampus Universitas Esa Unggul, yaitu Kampus Citra Raya, Kampus Kebon Jeruk, dan Kampus Harapan Indah, yang terhubung ke internet.  

 1. Koneksi ke Internet  
- Setiap kampus memiliki router yang terhubung ke internet.  
- Setiap router memiliki beberapa interface dengan IP yang berbeda:  
  - ether1: 10.10.10.2/24 (koneksi ke internet)  
  - ether2: 192.168.x.1/24 (koneksi ke jaringan internal)  
  - ether3: 176.10.10.1/24 (kemungkinan untuk koneksi antar kampus)  

 2. Kampus Citra Raya  
- Router KCR menghubungkan jaringan kampus ke internet dan jaringan internal.  
- Router KCR terhubung ke Lab Switch, yang mendistribusikan koneksi ke:  
  - Lab PC  
  - Access Point untuk perangkat mahasiswa  

 3. Kampus Kebon Jeruk  
- Router KJ memiliki fungsi serupa, tetapi terdapat tambahan Firewall sebelum koneksi masuk ke Lab Switch.  
- Firewall ini digunakan untuk mengontrol lalu lintas jaringan dan meningkatkan keamanan.  
- Setelah melewati firewall, Lab Switch mendistribusikan koneksi ke:  
  - Lab PC 
  - Access Point untuk perangkat mahasiswa  

 4. Kampus Harapan Indah  
- Router KHI langsung terhubung ke Lab Switch, tanpa firewall seperti di Kampus Kebon Jeruk.  
- Distribusi koneksi serupa dengan dua kampus lainnya:  
  - Lab PC  
  - Access Point untuk perangkat mahasiswa  

 5. Kesimpulan  
- Ketiga kampus memiliki topologi yang hampir serupa, dengan perbedaan utama pada Kampus Kebon Jeruk yang menggunakan Firewall tambahan.  
- Jaringan dikonfigurasi menggunakan Subnet 192.168.x.1/24 untuk jaringan internal, sementara subnet lain seperti 10.10.10.2/24 digunakan untuk koneksi eksternal ke internet.  
- Setiap kampus memiliki infrastruktur yang memungkinkan koneksi via kabel (Lab PC) maupun nirkabel (Access Point untuk perangkat mahasiswa).  
