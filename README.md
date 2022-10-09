# Clustering of Credit Risk with K-Means

## Summary:
Membuat Kredit Risk Clustering dengan Metode K-Means dan 10 Top Score pada Credit Risk Dataset

## Introduction: 
K-Means adalah salah satu algoritma yg bersifat unsupervised learning. (Unsupervised Learning adalah adalah salah satu tipe algoritma machine learning yg digunakan untuk menarik kesimpulan dari dataset. Metode ini hanya akan mempelajari suatu data berdasarkan clustering/pendekatan). K-Means memiliki fungsi untuk mengelompokkan data ke dalam data cluster. Algoritma ini dapat menerima data tanpa ada label kategori. K-Means algoritma juga termasuk metode non-hierarchy. Clustering algoritma K-Means memiliki tujuan untuk meminimalisir fungsi objective yang telah di set dalam proses clustering.

## Challenges:
### Menentukan nilai K terbaik untuk Clustering
### menentukan 10 Top Score

## Data Understanding : 
### Source Data: https://www.kaggle.com/datasets/laotse/credit-risk-dataset
### Dataset terdiri dari 12 kolom, 32581 baris, terdapat 4011 missing value, 165 duplicated value

## Data Dictionary:
### person_age				: usia (type : int)
### person_income  			: pendapatan tahunan (type : int)
### person_home_ownership	: kepemilikan rumah (type : object)
### person_emp_length		: lama kerja (dalam tahun) (type : float)
### loan_intent				: loan intent (type : object)
### loan_grade	 			: tingkat pinjaman (type : object)
### loan_amnt				: jumlah pinjaman (type : int)
### loan_int_rate				: suku bunga (type : float)
### loan_status				: Status pinjaman (0 tidak default 1 default) (type : int)
### loan_percent_income 		: percent pendapatan (type : float)
### cb_person_default_on_file : default historis (type : object)
### cb_person_cred_hist_length : panjang riwayat kredit (type : int)

## Data Preparation
### Python atau google colab untuk editor
### Packages : pandas, numpy, seaborn, skylearn cluster, matplotlib dll
<img width="532" alt="Screen Shot 2022-10-10 at 00 16 50" src="https://user-images.githubusercontent.com/112957682/194764806-dc9842fb-17a3-473c-8b04-4b5879530579.png">







