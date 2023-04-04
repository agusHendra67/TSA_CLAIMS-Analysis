# TSA_CLAIMS-Analysis


# Latar Belakang
TSA atau *Transportation Security Administration* adalah sebuah badan pemerintah dari departemen keamanan dalam negeri Amerika Serikat (USA) yang bertanggung jawab dalam masalah keamanan penerbangan. Klaim dapat diajukan jika penumpang terluka atau harta bendanya hilang atau rusak selama proses pemeriksaan di bandara. Banyak klaim yang masuk, tapi tidak semua klaim akan diproses dan disetujui.

## Pernyataan Masalah
TSA ingin mengetahui keputusan/penyelesaian akhir (*final settlement/Disposition*) apa yang harus diberikan dari sebuah klaim yang diajukan. Dimana ada tiga kategori untuk keputusan/penyelesaian akhir :

1. ***Approve in Full (Disetujui secara penuh)***   : klaim disetujui dan dana kompensasi diberikan secara penuh (full) sesuai dengan pengajuan klaim penumpang.
2. ***Settle (Disetujui secara parsial/sebagian)*** : klaim telah terselesaikan dengan persetujuan antara pihak agensi TSA dan penumpang. Dana kompensasi diberikan secara sebagian (partial)
3. ***Deny (Ditolak)***                             : klaim ditolak atau tidak disetujui.


Informasi ini diharapkan dapat membantu TSA untuk menekan biaya kompensasi dan waktu pengecekan klaim, mendeteksi adanya klaim fiktif atau palsu, memberikan evaluasi kepada bandara dalam hal penanganan klaim dan meningkatkan kualitas dengan membantu mengelompokkan klaim ke dalam keputusan akhir (*final settlement*) yang sesuai.

Sebagai seorang *data analyst*, saya akan mencoba menjawab pertanyaan berikut:

**Bagaimana karakteristik keputusan/penyelesaian akhir yang diambil terhadap klaim yang diajukan?**

# Data
Untuk menjawab pertanyaan di atas, saya akan menganalisa data klaim yang sudah dikumpulkan oleh TSA. Dataset dapat diakses [di sini](https://drive.google.com/drive/folders/13SAQcA3QZ2FBclO1iOW31otlnBXHytYk).

Dataset ini berisi informasi terkait jenis klaim, waktu kejadian dan pelaporan klaim, lokasi bandara, maskapai, status dan biaya klaim (dolar US). \
Ada 13 kolom di dalam data tsa_claims, yaitu

* Claim Number  : nomor id unik untuk setiap klaim
* Date Received : tanggal klaim diajukan
* Incident Date : tanggal kejadian tersebut terjadi
* Airport Code  : kode bandara dimana kejadian tersebut terjadi
* Airport Name  : nama bandara dimana kejadian tersebut terjadi
* Airline Name  : nama maskapai/penyedia penerbangan
* Claim Type    : tipe klaim yang diajukan
* Claim Site    : lokasi dimana klaim diajukan
* Item          : jenis benda yang di klaim
* Claim Amount  : jumlah dana (dolar US) klaim 
* Status        : status klaim yang diajukan (apakah sudah selesai, ditangguhkan , ditunda dll)
* Close Amount  : jumlah dana kompensasi penyelesaian akhir (settlement)
* Disposition   : status penyelesaian akhir ( *final settlement*) klaim

# Isi File

Ada beberapa tahapan yang dilakukan :

1. Data Understanding and Cleaning
2. Data Analysis
3. Kesimpulan dan Rekomendasi
