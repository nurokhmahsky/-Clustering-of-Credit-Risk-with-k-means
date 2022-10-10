# Clustering of Credit Risk with K-Means

## Summary:
Membuat Kredit Risk Clustering dengan Metode K-Means dan 10 Top Score pada Credit Risk Dataset

## Introduction: 
K-Means adalah salah satu algoritma yg bersifat unsupervised learning. (Unsupervised Learning adalah adalah salah satu tipe algoritma machine learning yg digunakan untuk menarik kesimpulan dari dataset. Metode ini hanya akan mempelajari suatu data berdasarkan clustering/pendekatan). K-Means memiliki fungsi untuk mengelompokkan data ke dalam data cluster. Algoritma ini dapat menerima data tanpa ada label kategori. K-Means algoritma juga termasuk metode non-hierarchy. Clustering algoritma K-Means memiliki tujuan untuk meminimalisir fungsi objective yang telah di set dalam proses clustering.

## Challenges:
Menentukan nilai K terbaik untuk Clustering
menentukan 10 Top Score

## Data Understanding : 
- Source Data: https://www.kaggle.com/datasets/laotse/credit-risk-dataset
- Dataset terdiri dari 12 kolom, 32581 baris, terdapat 4011 missing value, 165 duplicated value

## Data Dictionary:
- person_age                  : usia (type : int)
- person_income               : pendapatan tahunan (type : int)
- person_home_ownership       : kepemilikan rumah (type : object)
- person_emp_length           : lama kerja (dalam tahun) (type : float)
- loan_intent                 : loan intent (type : object)
- loan_grade                  : tingkat pinjaman (type : object)
- loan_amnt                   : jumlah pinjaman (type : int)
- loan_int_rate				        : suku bunga (type : float)
- loan_status				          : Status pinjaman (0 tidak default 1 default) (type : int)
- loan_percent_income 		    : percent pendapatan (type : float)
- cb_person_default_on_file   : default historis (type : object)
- cb_person_cred_hist_length  : panjang riwayat kredit (type : int)

## Data Preparation
- Python atau google colab untuk editor
- Packages : pandas, numpy, seaborn, skylearn cluster, matplotlib dll
<img width="532" alt="Screen Shot 2022-10-10 at 00 16 50" src="https://user-images.githubusercontent.com/112957682/194764806-dc9842fb-17a3-473c-8b04-4b5879530579.png">

##	Data Cleansing
- Missing Value
<img width="697" alt="Screen Shot 2022-10-10 at 22 19 46" src="https://user-images.githubusercontent.com/112957682/194875845-d0fcf5f8-13c6-4c9a-b345-ab5aa4de0cf2.png">

- Duplicated Value
  Terdapat 165 value, lalu drop duplicated value
- Outlier 
![outlier age](https://user-images.githubusercontent.com/112957682/194936742-62bdbc80-f8db-4ba9-89e6-166c93e267be.png)
  outlier "person_age" dengan age > 60 tahun


## EDA (Exploratory Data Analysis)








