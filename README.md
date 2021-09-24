# ScikitLearnGroup_JC_DS_BDG_07_FinalProject
**Business Understanding**

## **Business**  **and Problem Statement**



## **Business Objectives**

Tujuan bisnis yang akan dicanangkan adalah sebagai berikut :

- Memprediksi harga mobil berdasarkan spesifikasi mobil.
- Menyediakan Informasi mengenai batas atas dan batas bawah dari harga mobil agar dapat meraih keuntungan namun masih bersaing dengan harga pasar.

## **Data Availability**

Data yang dimiliki hanya terbatas mobil yang dijual terlepas dari apakah mobil tersebut telah terjual maupun tidak. Kami akan menggunakan pola dari brand, model, dan spesifikasi mobil dengan harga jualnya sebagai blablabla.

## **Analytic Approach**

Machine Learning dengan tipe Supervised Learning Regression menjadi metode kami untuk memprediksi harga mobil. Data yang sudah dibersihkan akan dibagi menjadi 3 yaitu : Data Train, Data Validation, dan Data Test. Nantinya Data Test akan diambil sebagian sebagai tolak ukur pengaruh model terhadap keuntungan perusahaan. Untuk pelatihan dan validasi akan diiterasi sebanyak 5 kali agar dapat mendapatkan hasil yang konsisten. Evaluasi dilakukan dengan membandingkan R Square antar model. Setelah diketahui model-model terbaik, akan dilakukan hyperparameter tuning dengan menggunakan 2 metode yaitu GridSearch dan RandomSearch agar dapat meraih hasil prediksi yang optimal.

Kekeliruan dalam prediksi dapat menyebabkan dampak seperti berikut :

- Ketika hasil prediksi yang dilakukan jauh dibawah harga pasar. Maka perusahaan berpotensi untuk kehilangan keuntungan karena sesungguhnya mobil dapat dijual dengan harga yang lebih tinggi.
- Ketika hasil prediksi yang dilakukan melebihi harga pasar. Maka mobil yang tersebut mempunyai peluang terjual yang sangat sedikit.

# **Data Understanding**

Kami menggunakan Dataset &quot;100,000 UK Used Car Data set&quot; yang ada di Kaggle. Dataset tersebut berisi data mobil yang dijual yang ada di UK dari tahun 1970 hingga 2020. Dataset tersebut mempunyai 9 variabel termasuk 1 label &quot;price&quot; di dalamnya. Berikut adalah detail dari variabel yang ada :

| **Attribute** | **Data Type** | **Description** |
| --- | --- | --- |
| brand | string | Nama brand mobil. |
| model | string | Model dari brand terkait. |
| year | interger | Tahun pembuatan mobil. |
| transmission | string | Jenis transmisi yang digunakan mobil. |
| mileage | interger | Jarak tempuh mobil. |
| fueltype | string | Jenis bahan bakar yang dibutuhkan mobil. |
| enginesize | float | Ukuran mesin dalam liter (L) |

Dan berikut adalah rincian dari label dataset :

Nama : price <br>
Tipe Data : float <br>
Deskripsi : Harga mobil satuan.
