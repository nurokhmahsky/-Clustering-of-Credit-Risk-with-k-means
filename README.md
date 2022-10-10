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
### Univariate Analysisis 
  - Boxplot Univariate Numericals
![boxplot univariate numerik](https://user-images.githubusercontent.com/112957682/194946254-90939d64-8011-4d3c-98a5-489d9f56471e.png)
  - Countplot Univariate Categoricals
![univariate countplot categorik](https://user-images.githubusercontent.com/112957682/194947042-dcd389c6-940c-4178-a6f2-9923bf8e74b9.png)

### Bivariate Analysis
- Lineplot Analysis Feature 'person_age, loan_amnt, cb_person_cred_hist_length'![bivariate](https://user-images.githubusercontent.com/112957682/194948176-ed316fc8-59c0-45d1-aafb-699e0819546d.png)
- Dari gambar diatas dapat disimpulkan bahwa:
1. perbedaan 'loan_status' yg lumayan tinggi pada 'person_age' > 60 tahun
2. perbedaan yg tinggi juga antara 'cb_person_cred_hist_length' dan 'person_age' dengan value sekitar 50-70
3. mengalami peningkatan value 'loan_amnt' pada 'cb_person_cred_hist_length' >15

- Heatmap Correlation feature 'person_age, loan_amnt, cb_person_cred_hist_length'![heatmap correlation](https://user-images.githubusercontent.com/112957682/194948841-6348b357-8b32-4aac-acaa-aa63cdc9d145.png)
- Dari hasil korelasi heatmap diatas dapat dilihat ada korelasi positif antara feature 'person_age' dan 'cb_person_cred_hist_lenght'
- Distplot Distribution feature 'person_age , loan_percent_income, person_emp_length'
![distplot distribution](https://user-images.githubusercontent.com/112957682/194949514-ef86eedb-2ed2-4aba-80c5-3f48814722e4.png)
- Distplot Log Transformation feature (person_age, loan_percent_income, person_emp_length) untuk menghilangkan Skewness ![log trans](https://user-images.githubusercontent.com/112957682/194950151-5de54cbe-d90c-47ce-99d3-b9add5d891d9.png)
- K-Means Elbow Method Clustering untuk menentukan value K optimal![KMeans](https://user-images.githubusercontent.com/112957682/194951262-a47e6065-f9e7-428f-b10f-fb6465fb8975.png)
- Cluster dengan Value K = 6
-  3D Scatter Plot Cluster 6 ![newplot](https://user-images.githubusercontent.com/112957682/194952100-24e4b5f0-d629-45aa-bb31-b67f74112577.png)
- Pie Chart Percentage Size of Clustering ![newplot (1)](https://user-images.githubusercontent.com/112957682/194953077-42931806-be5a-4ca3-bc86-68f4b91ec83a.png)







