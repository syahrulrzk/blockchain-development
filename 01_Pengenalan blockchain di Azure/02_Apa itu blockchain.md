# Apa itu blockchain?
Blockchain adalah teknologi penyimpanan catatan dan penegakan kontrak yang menggunakan kriptografi untuk menyulitkan perubahan riwayat sebelumnya. Ini memungkinkan peserta berbagi aliran kerja dengan melacak perubahan pada ledger bersama.

Dalam skenario es krim, bagaimana kita menemukan apakah ada masalah kualitas makanan atau keamanan yang disebabkan oleh penyimpanan suhu yang tidak tepat selama pengiriman? Kita perlu melacak pihak yang bertanggung jawab dan suhu serta menyimpan log perubahan.

# Mengapa tidak menggunakan database terpusat?
Kita bisa menggunakan database terpusat yang digunakan semua peserta untuk melacak pengiriman. Dalam banyak skenario, database terpusat adalah solusi yang tepat. Misalkan kita memiliki database terpusat yang menyimpan rincian tentang pengiriman dan siapa yang saat ini bertanggung jawab. Dalam skenario kita, kita bisa mendapati peternak, pengirim, pabrik, dan peritel menggunakan database terpusat yang sama.

![image](https://github.com/user-attachments/assets/a612ecab-8581-4e9c-958b-b2b8d73587de)

Manfaat dari database terpusat adalah kemudahan untuk mengontrol akses dan konsistensi. Setiap orang menggunakan database yang sama, dan ada otoritas tepercaya yang mengontrol akses. Karena hanya ada satu database, semua peserta menggunakan kumpulan data yang sama. Semua peserta perlu memercayai database sudah benar, dan dengan ekstensi, mereka perlu mempercayai pemilik database untuk tidak memodifikasi data historis karena alasan apa pun.

Bagaimana jika skenario kita tidak memungkinkan otoritas pusat yang tepercaya? Bagaimana jika tidak ada perusahaan yang ingin bertanggung jawab untuk menghosting database terpusat? Mungkin persyaratan untuk integrasi sistem dengan setiap sistem peserta tidak dapat dipenuhi.

# Database terdistribusi
Bagaimana jika setiap peserta bisa memiliki salinan database mereka sendiri? Database terdistribusi menggunakan beberapa salinan database, dan perubahan disinkronkan. Dalam skenario kita, kita bisa mendapati peternak, pengirim, pabrik, dan peritel menggunakan database terdistribusi milik mereka sendiri.

![image](https://github.com/user-attachments/assets/e239fcbf-a64a-4293-98d0-e0d5192e7042)

Manfaat dari database terdistribusi adalah bahwa setiap peserta memiliki salinan database. Dalam kebanyakan kasus, lebih mudah untuk mengontrol akses dan mengintegrasikan sistem Anda serta memproses dalam salinan database Anda sendiri. Namun, menyinkronkan perubahan pada setiap database diperlukan. Menangani kegagalan dan konflik dapat menambah kompleksitas dan masalah integritas data.

# Ledger terdistribusi

Teknologi Blockchain disebut sebagai ledger terdistribusi. Sama seperti ledger akuntansi, ledger terdistribusi adalah riwayat transaksi. Setiap transaksi dalam ledger memengaruhi kondisi akhir.

Jaringan blockchain yang didistribusikan di antara peserta disebut jaringan konsorsium. Jaringan konsorsium memberikan visibilitas kepada setiap mitra untuk setiap transaksi yang terjadi di jaringan.

![image](https://github.com/user-attachments/assets/36b34298-6140-4cbf-8a32-3a114eef9f59)

Blockchain menggunakan aturan konsensus untuk memastikan data konsisten di seluruh node. Blockchain juga menggunakan kriptografi untuk memungkinkan peserta memercayai data. Secara khusus, blockchain mencegah setiap peserta individu atau minoritas peserta memodifikasi riwayat. Karena blockchain terdesentralisasi, solusi yang dapat menggunakan database terdesentralisasi akan sangat sesuai. Misalnya, Anda memiliki persyaratan untuk mendukung beberapa perusahaan tanpa otoritas pusat karena alasan biaya, kontrol, atau dianggap menjadi satu titik kegagalan.


