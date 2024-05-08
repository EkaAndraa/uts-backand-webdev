UTS BACK-END WEB DEVELOPMENT

Nama:Komang eka andra tri dharma
Nim:230010087

PENJELASAN MENGENAI KONFIGURASI SISTEM

1. Direktori config
database.php: File ini merupakan inti dari konfigurasi basis data. Menggunakan PHP Data Objects (PDO), file ini menetapkan parameter penting seperti host, nama basis data, pengguna, dan kata sandi. Didesain untuk mengelola koneksi basis data secara aman, file ini juga dilengkapi dengan penanganan eksepsi untuk mengantisipasi dan menyelesaikan kesalahan koneksi.
2. Direktori public
index.php: Sebagai pintu masuk aplikasi, file ini diakses pertama kali oleh pengunjung situs. Saat ini, file ini hanya menampilkan header "XYZ Sales API End Point", yang menandakan titik akses API untuk aplikasi penjualan XYZ.
3. Direktori src
3.1. Sub-direktori Controller
CustomerController.php: Bertugas mengatur operasi CRUD untuk data pelanggan. File ini menyediakan metode untuk mengakses, menambah, memperbarui, dan menghapus informasi pelanggan, bekerja sama dengan model Customers.php.
PurchaseController.php: Mengelola operasi CRUD untuk transaksi pembelian. File ini memfasilitasi akses dan manipulasi data pembelian, berkoordinasi dengan model Purchases.php.
SalesController.php: Menangani operasi CRUD untuk data penjualan. File ini memungkinkan pengambilan dan perubahan informasi penjualan, berinteraksi dengan model Sales.php.
Semua controller ini dirancang untuk menerima dan memproses permintaan HTTP sesuai dengan fungsi yang ditentukan.

3.2. Sub-direktori Model
Customers.php: Bertanggung jawab atas eksekusi query terkait data pelanggan, berdasarkan instruksi dari CustomerController.php, dan menghubungkan aplikasi dengan basis data pelanggan.
Purchases.php: Melaksanakan query untuk data pembelian, menerima arahan dari PurchaseController.php, dan memastikan koneksi yang lancar dengan basis data pembelian.
Sales.php: Menjalankan query yang berkaitan dengan data penjualan, sesuai dengan perintah dari SalesController.php, dan menjaga integrasi dengan basis data penjualan.
Setiap model ini mengimplementasikan serangkaian query untuk mengambil, memasukkan, memperbarui, dan menghapus data, memastikan aplikasi dapat berinteraksi dengan basis data secara efisien dan efektif.

REFLEKSI DIRI
Sebagai pengembang project ini, saya ingin berbagi beberapa refleksi tentang tantangan dan solusi yang saya hadapi selama pengembangan. Saya menghadapi berbagai tantangan yang tidak hanya menguji kemampuan teknis saya, tetapi juga ketahanan dan kemampuan untuk beradaptasi.

TANTANGAN YG DIHADAPI
Salah satu tantangan terbesar adalah implementasi operasi CRUD yang efisien. Mengkoordinasikan antara Controllers dan Models untuk memastikan bahwa data diolah dengan benar merupakan proses yang kompleks.sesuatu yang belum pernah saya kerjakan sebelumnya, dan pada awalnya, saya merasa kewalahan. Saya juga mengalami kesulitan dalam mengelola ketergantungan antara kelas-kelas dan memastikan koneksi database 

CARA MENGATASI TANTANGAN 
Untuk mengatasi tantangan CRUD, saya menghabiskan waktu untuk mempelajari dokumentasi PHP dan MySQL secara mendalam, serta mencari sumber daya tambahan seperti tutorial dan forum komunitas. Praktik ini memungkinkan saya untuk memperbaiki bug dan meningkatkan efisiensi kode.Saya juga mencari pembelajaran dantutorial di YouToub