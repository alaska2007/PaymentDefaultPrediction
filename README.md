# PaymentDefaultPrediction
Final Project Kelompok 8 (INFINITY) - Rakamin Batch 21

FINAL PROJECT KELOMPOK 8 (INFINITY)
Nama Kelompok :

1. Alaska Napitupulu, 
2. Rafsanjani Lestari Negara, 
3. Ukhti Aprillia Vanny, 
4. Ike Setyawati, 
Dataset : https://www.kaggle.com/reverie5/av-janata-hack-payment-default-prediction

Folder Stage 0 :
Tahap Preparation. Pada Stage 0 kami menjelaskan Role, Problem Statement, Goal and Objective, dan Business Metrics .

-Problem Statement
Bank Of Taiwan memiliki produk pinjaman kartu kredit jangka pendek dimana saat ini terdapat debitur(cardholder) yang lalai dalam melakukan pembayaran setiap bulannya baik pembayaran dibawh minimum payment maupun keterlambatan dalam pembayaran. Kelalaian debitur (cardholder) mengakibatkan menurunnya profit bank karena banyaknya piutang bank yang tak tertagih. Oleh karena itu kami sebagai bussdev akan melakukan upaya peningkatan baik dengan pemberian keringanan pembayaran ataupun pemberian perpanjangan waktu supaya debitur tetap dapat melakukan kewajibnnya untuk membayar.
Data yang kami sajikan berisikan id nasabah, pendidikan, status menikah, usia nasabah, history pembayaran dan history keterlambatan bayar.

-Goal

Mendeteksi adanya kemungkinan cardholder yang akan gagal bayar.
Menurunkan tingkat default
Membantu bank untuk tetap mendapatkan profit.
Informasi lebih lengkap mengenai stage 0 bisa dilihat di folder Stage 0

Folder Stage 1 :
Tahap EDA, Insights dan Visualization.
Dari tahap EDA kami mendapatkan beberapa point :

semua fitur memiliki tipe kolom yang sesuai begitu juga isinya
tidak memiliki missing value
beberapa features memiliki nilai mean>median dan selisih percentil 75 dengan max sangat jauh.
Dari Visualization kami mendapatkan beberapa point :

semua numerical data tampak skew ke kanan
berdasarkan visualisasi blotplot terdapat beberapa feature yang memiliki outliers
korelasi antara features(LIMIT_BAL,Pay_0,Pay_2,Pay_3,Pay_4,Pay_5,Pay_6 dan target (default_payment_next_month) memiliki korelasi positif lemah
customer yang default dan tidak default memiliki rata-rata limit balance dimana customer default yang lebih rendah.
Kemampuan bayar customer default rata-rata hanya 1/2 kali dari customer yang tidak default
Point-point lainnya bisa dilihat di folder Stage 1

Folder Stage 2 :
Tahap Data Pre-processing. Pada Stage 2 ini kami melakukan Data Cleansing dan Feature Engineering
Data cleansing, mendapat beberapa point :

Tidak ada missing value
Tidak ada duplicated data
Terdapat outliers dan akan dihandling dengan z-score
Features Transformation
Features encoding = SEX and EDUCATION(label encod) sedangkan MARRIAGE dan PAY_0 – PAY_6 (OneHotEncoding)
Handle class imbalance menggunakan Z-score
Pada data Feature Engineering kami tidak melakukan Feature selection maupun Feature extraction
