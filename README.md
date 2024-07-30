# 🚩 Project Name: Bank Costumer Churn Rate Analysis

🙋🏻‍♂️ Project Owner: Ahmad Dani Rifai  
🏁 Date Finished: Juni 2024  
📞 Contact: [LinkedIn](https://www.linkedin.com/in/ahmad-dhani-0b8b6a22b/); [E-mail](adhani866@gmail.com)

---

## Objectives

Mengelompokkan pelanggan berdasarkan pola penggunaan dan kebiasaan transaksi mereka. Dengan melakukan klasterisasi, perusahaan kartu kredit dapat mengidentifikasi segmen-segmen pelanggan yang memiliki karakteristik serupa, seperti frekuensi pembelian, penggunaan pembayaran tunai di muka, dan tingkat pembayaran minimum. Hal ini memungkinkan perusahaan untuk merancang strategi pemasaran yang lebih efektif, memberikan penawaran yang lebih tepat sasaran, dan meningkatkan layanan pelanggan. Selain itu, klasterisasi juga dapat membantu dalam mendeteksi perilaku anomali atau potensi risiko, sehingga perusahaan dapat mengambil tindakan pencegahan yang sesuai.

- Memperoleh data menggunakan BigQuery

- Mempersiapkan data untuk digunakan dalam Clustering

- Memahami konsep Clustering dengan menggunakan Scikit-Learn

- Mengimplementasikan Clustering pada data yang di yang sudah didapat dari Bigquery

---

## Dataset

| **Column Name**                | **Data Type** | **Description**                                                                                                                    |
| ------------------------------ | ------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| CUSTID                         | Object        | Identifikasi pemegang kartu kredit                                                                                                 |
| BALANCE                        | Float         | Jumlah saldo yang tersisa di akun untuk melakukan pembelian                                                                        |
| BALANCEFREQUENCY               | Float         | Seberapa sering saldo diperbarui, nilai antara 0 dan 1 (1 = sering diperbarui, 0 = tidak sering diperbarui)                        |
| PURCHASES                      | Float         | Jumlah pembelian yang dilakukan dari akun                                                                                          |
| ONEOFFPURCHASES                | Float         | Jumlah maksimum pembelian yang dilakukan dalam satu kali transaksi                                                                 |
| INSTALLMENTSPURCHASES          | Float         | Jumlah pembelian yang dilakukan dengan cicilan                                                                                     |
| CASH ADVANCE                   | Float         | Uang muka yang diberikan oleh pengguna                                                                                             |
| PURCHASESFREQUENCY             | Float         | Seberapa sering pembelian dilakukan, nilai antara 0 dan 1 (1 = sering membeli, 0 = tidak sering membeli)                           |
| ONEOFFPURCHASESFREQUENCY       | Float         | Seberapa sering pembelian dilakukan dalam satu kali transaksi, nilai antara 0 dan 1 (1 = sering membeli, 0 = tidak sering membeli) |
| PURCHASESINSTALLMENTSFREQUENCY | Float         | Seberapa sering pembelian dengan cicilan dilakukan, nilai antara 0 dan 1 (1 = sering dilakukan, 0 = tidak sering dilakukan)        |
| CASHADVANCEFREQUENCY           | Float         | Seberapa sering uang muka dibayar, nilai antara 0 dan 1 (1 = sering dibayar, 0 = tidak sering dibayar)                             |
| CASHADVANCETRX                 | Integer       | Jumlah transaksi yang dilakukan dengan "uang muka"                                                                                 |
| PURCHASESTRX                   | Integer       | Jumlah transaksi pembelian yang dilakukan                                                                                          |
| CREDIT LIMIT                   | Float         | Batas kredit kartu untuk pengguna                                                                                                  |
| PAYMENTS                       | Float         | Jumlah pembayaran yang dilakukan oleh pengguna                                                                                     |
| MINIMUM_PAYMENTS               | Float         | Jumlah pembayaran minimum yang dilakukan oleh pengguna                                                                             |
| PRCFULLPAYMENT                 | Float         | Persentase pembayaran penuh yang dilakukan oleh pengguna                                                                           |
| TENURE                         | Integer       | Masa layanan kartu kredit untuk pengguna                                                                                           |

---

## Problems

Membuat model clustering untuk melakukan Customer Segmentation dari data kartu kredit sebuah bank dibawah ini. Data ini merupakan data informasi penggunaan kartu kredit selama 6 bulan terakhir.

---

## Daftar konten di bawah ini:

1.  Perkenalan

    > Bab pengenalan harus diisi dengan identitas, gambaran besar dataset yang digunakan, dan _objective_ yang ingin dicapai.

2.  Query SQL

    > Tulis query yang telah dibuat untuk mengambil data dari Google Cloud Platform di bagian ini.

3.  Import Libraries

    > _Cell_ pertama pada _notebook_ **harus berisi dan hanya berisi** semua _library_ yang digunakan dalam _project_.

4.  Data Loading

    > Bagian ini berisi proses penyiapan data sebelum dilakukan eksplorasi data lebih lanjut. Proses Data Loading dapat berupa memberi nama baru untuk setiap kolom, mengecek ukuran dataset, dll.

5.  Exploratory Data Analysis (EDA)

    > Bagian ini berisi explorasi data pada dataset diatas dengan menggunakan query, grouping, visualisasi sederhana, dan lain sebagainya.

6.  Feature Engineering

    > Bagian ini berisi proses penyiapan data untuk proses pelatihan model, seperti transformasi data (normalisasi, encoding, dll.), dan proses-proses lain yang dibutuhkan.

7.  Model Definition

    > Bagian ini berisi cell untuk mendefinisikan model. Jelaskan alasan menggunakan suatu algoritma/model, hyperparameter yang dipakai, jenis penggunaan metrics yang dipakai, dan hal lain yang terkait dengan model.

8.  Model Training

    > Cell pada bagian ini hanya berisi code untuk melatih model dan output yang dihasilkan. Lakukan beberapa kali proses training dengan hyperparameter yang berbeda untuk melihat hasil yang didapatkan. Analisis dan narasikan hasil ini pada bagian Model Evaluation.

9.  Model Evaluation

    > Pada bagian ini, dilakukan evaluasi model yang harus menunjukkan bagaimana performa model berdasarkan metrics yang dipilih. Hal ini harus dibuktikan dengan visualisasi tren performa dan/atau tingkat kesalahan model. **Lakukan analisis terkait dengan hasil pada model dan tuliskan hasil analisisnya**.

10. Model Saving

    > Pada bagian ini, dilakukan proses penyimpanan model dan file-file lain yang terkait dengan hasil proses pembuatan model.

11. Model Inference

    > Model yang sudah dilatih akan dicoba pada data yang bukan termasuk ke dalam train-set. Data ini harus dalam format yang asli, bukan data yang sudah di-scaled.

12. Pengambilan Kesimpulan
    > Pada bagian terakhir ini, **harus berisi** kesimpulan yang mencerminkan hasil yang didapat dengan _objective_ yang sudah ditulis di bagian pengenalan.

---
