# Cara kerja blockchain

Sekarang setelah mengetahui dasar-dasar blockchain, mari kita lihat cara kerjanya di belakang layar. Informasi ini akan membantu Anda memutuskan apakah blockchain berfungsi untuk skenario Anda.

# Bagaimana data didistribusikan?

Dalam skenario kita, ada beberapa perusahaan. Kita bisa memiliki database terpusat di perusahaan pengolahan susu. Namun, tidak ada satu pun peserta yang ingin menjadi otoritas pusat. Kita dapat menggunakan ledger yang didistribusikan blockchain. Menggunakan blockchain akan menghapus kebutuhan akan otoritas pusat. Juga, setiap peserta dengan node blockchain memiliki salinan ledger sehingga mereka dapat melakukan audit dan integrasi sendiri dengan sistem mereka. Namun, tidak ada persyaratan bagi setiap perusahaan untuk memiliki node mereka sendiri. Mitra dapat berbagi simpul.

Setiap node terhubung ke node lain menggunakan jaringan blockchain. Misalnya, peternakan Dalia Pelayo, pabrik es krim, dan toko es krim masing-masing memiliki node yang mereka kelola. Contoso West dan Contoso East adalah mitra terpisah yang memiliki perusahaan induk yang sama. Contoso memiliki satu node. Tidak perlu ada hubungan satu ke satu dari node dengan perusahaan.

![image](https://github.com/user-attachments/assets/261bbed7-977a-4999-af98-ae976516fad3)

# Mengubah status
Data dalam blockchain menunjukkan status. Itu sebabnya token digital seperti cryptocurrency cocok untuk blockchain. Jika kita berpikir tentang kepemilikan mata uang fisik, sebuah koin hanya bisa berada di saku satu orang pada satu waktu. Jika koin ada di saku Anda, status kepemilikannya adalah milik Anda. Jika Anda memberikan koin kepada teman Anda, statusnya berubah menjadi teman Anda yang memiliki koin. Dalam skenario kita, pengiriman bergerak melalui rantai pasokan. Tanggung jawab atas produk harus dialihkan. Data di mana kami tertarik adalah pihak yang bertanggung jawab, suhu, dan jika produk sesuai.

Blockchain menggunakan transaksi untuk mengubah status data dari satu nilai ke nilai lainnya. Misalnya, kita perlu tahu apakah es krim disimpan di bawah titik beku. Dalam pengiriman es krim, sensor suhu melaporkan suhu secara berkala. Suhu yang dilaporkan adalah transaksi yang dikirim ke simpul transaksi blockchain.

![image](https://github.com/user-attachments/assets/4c2382e7-d471-4877-bb58-5a71925b7014)

Dalam skenario es krim, ketika pengiriman dikirim melalui rantai pasokan, transaksi dikirim setiap kali status berubah. Misalnya, ilustrasi menunjukkan transaksi untuk pengiriman biasa ke pabrik es krim. Setiap transaksi akan mengubah entah itu pihak yang bertanggung jawab ataupun suhu. Status ledger saat ini adalah transaksi yang diterapkan secara berurutan.

![image](https://github.com/user-attachments/assets/09e5cb7a-d28f-422b-a2d3-e941b736ddfb)

Saat mengirim transaksi, Anda mengirimkannya ke node transaksi blockchain. Anggap saja Peternakan Dalia Pelayo mengirimkan kiriman susu menggunakan Pengiriman Contoso West. Sistem pengiriman Dalia Pelayo Farms mengirimkan transaksi ke simpul blockchain mereka. Transaksi memperbarui tanggung jawab pengiriman dari peternak ke Pengiriman Contoso West.

![image](https://github.com/user-attachments/assets/646b0e9a-0bce-4eff-8d5a-b77c7b12219f)

Blockchain mengirimkan transaksi ke seluruh jaringan blockchain. Setiap node mendapatkan salinan transaksi.

![image](https://github.com/user-attachments/assets/a02b07f2-91dd-4112-9928-e2c8a347d9f9)

Setiap simpul memproses transaksi, tetapi masih memerlukan validasi menggunakan mekanisme konensius. Konsensus memungkinkan konsistensi dan kepercayaan untuk ledger terdistribusi.

# Bagaimana Anda bisa percaya data ledger konsisten?
Dalam jaringan terdistribusi, sulit untuk menentukan apa yang benar, karena perubahan data harus terjadi di semua simpul. Apa yang terjadi jika node pabrik es krim tidak mendapatkan transaksi pengiriman? Bagaimana mereka tahu jika susu telah dikirim dari peternakan? Bagaimana jika truk pendingin perusahaan pengiriman bermasalah dan susu basi? Mungkinkah perusahaan pengiriman memodifikasi ledger mereka untuk menghindari tanggung jawab?

Blockchain menggunakan mekanisme konsensus untuk memvalidasi dan menyetujui data di semua node blockchain. Konsensus menyediakan cara bagi semua node terdesentralisasi untuk memiliki status yang sama. Saat mentransfer nilai atau tanggung jawab, urutan menjadi penting. Misalnya, jika Anda mentransfer kepemilikan mobil kepada teman Anda, Anda tidak bisa juga mentransfer kepemilikan ke kolega di tempat kerja. Masalah ini dikenal sebagai masalah pengeluaran ganda, yang diselesaikan konensus. Konsensus memastikan urutan yang benar pada transaksi dan integritas blockchain. Sebagai bagian dari konsensus, sekelompok transaksi divalidasi sebagai blok dan jaringan harus setuju apakah blok sebaiknya dimasukkan dalam blockchain.

![image](https://github.com/user-attachments/assets/f0be7d78-c5c6-4fbc-90f5-dcec6914c6ef)

Ada beberapa algoritma konsekuensi blockchain, termasuk bukti kerja, bukti pasak, dan bukti otoritas. Setiap algoritma memecahkan konsistensi dengan cara yang berbeda. Secara sederhana, konsensus menyediakan cara untuk ledger terdistribusi memiliki status yang sama.

# Apa itu blok?
Blok adalah kluster data dalam blockchain yang menyimpan informasi transaksi. Jumlah transaksi dalam blok biasanya berbasis waktu. Misalnya, ilustrasi berikut menunjukkan blok yang berisi transaksi yang terjadi dalam 10 menit terakhir:

![image](https://github.com/user-attachments/assets/39be4f6d-90b5-40cc-8d13-ad793225a655)

Melalui konsensus, blok yang divalidasi ditambahkan ke blockchain di setiap node. Karena semua node memiliki blok yang sama dalam rantai, ledger pun konsisten di seluruh jaringan. Alhasil, semua node berisi data tervalidasi yang sama dalam urutan yang disepakati.

# Bagaimana Anda bisa percaya bahwa ledger tidak dapat diubah?
Anda akan berpikir bahwa jika Anda memiliki kontrol ledger di simpul Anda, Anda hanya dapat mengubah data dalam salinan Anda. Bagaimana bisa ledger tidak berubah?

Blockchain menggunakan hash kriptografi untuk membuat tautan antar blok. Dengan menautkan blok, urutan transaksi dapat disepakati melalui algoritma konsensus. Hash kriptografi adalah algoritma yang memetakan data dengan ukuran arbitrer ke sedikit representasi ukuran tetap. Anda dapat menganggapnya sebagai sidik jari digital. Bitcoin menggunakan algoritma hash SHA-256. Jika Anda menggunakan fungsi hash SHA-256 pada dokumen halaman 100, output fungsi adalah nilai hash 256-bit. Jika Anda hanya mengubah satu karakter dalam dokumen dan meregenerasi hash, outputnya adalah nilai hash 256-bit yang berbeda. Sekarang, bayangkan jika kita menggunakan blok sebagai input ke fungsi hash. Outputnya adalah nilai hash yang unik untuk data dalam blok.

![image](https://github.com/user-attachments/assets/1bb15884-2774-47ce-82d0-8a4f6a329d68)

Blockchain menggunakan hash untuk mendeteksi apakah ada perubahan yang telah dilakukan pada blok. Dengan menyertakan nilai hash blok sebelumnya saat membuat hash blok berikutnya, blok dirantai bersama-sama melalui hash.

![image](https://github.com/user-attachments/assets/cfc2aebf-baff-4197-9d77-fd5af8783a48)

Blockchain memberikan kepercayaan dengan menggunakan hash untuk membuktikan riwayat data tidak berubah. Dengan menyertakan hash blok sebelumnya saat membuat blok baru, rantai transaksi yang tidak dapat diubah dibuat secara berurutan.

![image](https://github.com/user-attachments/assets/5039ef1a-ee30-4ef1-8a21-961cb7cda7c0)

Jika ada blok yang dimodifikasi dalam rantai, blok selanjutnya memiliki hash yang berbeda. Akibatnya, validasi menemukan perbedaan.

# Logika tepercaya
Blockchain memungkinkan kami menyimpan data yang konsisten dan tepercaya. Bagaimana kita menambahkan logika yang menjalankan hal yang sama di setiap node?

Dalam skenario kita, kita membutuhkan logika untuk mentransfer tanggung jawab produk dari satu peserta ke peserta lain. Kita juga perlu menggunakan data dari sensor suhu IoT untuk mengetahui apakah suhu terlalu tinggi.

Aplikasi terdesentralisasi (DApp) adalah aplikasi pada sistem komputasi terdistribusi. Dalam modul ini, kami berfokus pada penggunaan protokol blockchain Ethereum. DApp Ethereum disebut kontrak pintar. Kontrak pintar berisi logika yang dijalankan sebagai bagian dari transaksi. Di Ethereum, Anda memprogram logika menggunakan bahasa pemrograman yang disebut Solidity.

Kontrak pintar diterapkan ke blockchain dan dirujuk oleh alamat. Untuk menggunakan kontrak pintar, Anda membuat instans. Instans kontrak pintar berisi data status dan logika program. Dalam skenario kami, instans kontrak pintar berisi data seperti peserta yang bertanggung jawab, lokasi, dan jika suhu produk tidak sesuai. Kita dapat menjalankan fungsi untuk mentransfer tanggung jawab atau menerima telemetri suhu untuk instans.

![image](https://github.com/user-attachments/assets/b768748f-c156-465a-8c1c-1c82a84f440d)

Ketika tanggung jawab produk ditransfer ke pihak lain, transaksi dijalankan. Logika kontrak pintar memperbarui data status. Dalam skenario es krim kita, sistem pengiriman pabrik es krim menciptakan instans kontrak pintar untuk pengiriman es krim baru. Sistem pengiriman pabrik mengirimkan transaksi yang memanggil fungsi TransferResponsibility untuk mentransfer tanggung jawab pengiriman ke pengiriman Contoso East. Jaringan blockchain mengirimkan transaksi ke semua node. Logika kontrak pintar dijalankan di setiap simpul.

![image](https://github.com/user-attachments/assets/5f27c34e-61c0-4fd2-85b3-70f70ef4f36d)

Bagaimana jika selama pengiriman, unit pendingin gagal dan suhu es krim berada di atas pembekuan? Sensor suhu IoT memantau suhu es krim dan mengirim transaksi secara berkala. Jika suhu di atas membeku, logika kontrak pintar menandai pengiriman sebagai tidak patuh.

![image](https://github.com/user-attachments/assets/6182d2f3-8d43-4d07-9197-6a1eed507892)

Karena transaksi termasuk dalam rantai blok, ada catatan yang tidak dapat diubah ketika pengiriman menjadi tidak patuh. Toko es krim dapat menolak pengiriman dan dapat menghindari masalah keamanan makanan.

Sama seperti data di blockchain, kontrak pintar tidak dapat diubah. Setelah disebarkan, logika tidak dapat diubah. Oleh karena itu, Anda bisa yakin bahwa logika kontrak pintar selalu menjalankan yang sama di semua node. Setiap perubahan kode mengharuskan kontrak pintar baru diterapkan di alamat baru.
