# Tugas_Praktikum_023_043
# Klasifikasi Diabetic Retinopaty Menggunakan CNN

# Overview Jurnal
1. Jurnal Referensi
Jurnal referensi pada projek ini berjudul Deep Learning untuk Klasifikasi Diabetic Retinopathy menggunakan Model EfficientNet
http://dx.doi.org/10.26760/elkomika.v8i3.693

Diabetic Retinopathy merupakan penyakit yang dapat mengakibatkan kebutaan 
mata yang disebabkan oleh adanya komplikasi penyakit diabetes melitus. Oleh 
karena itu mendeteksi secara dini sangat diperlukan untuk mencegah bertambah 
parahnya penyakit tersebut. Penelitian ini merancang sebuah sistem yang dapat 
mendeteksi Diabetic Retinopathy berbasis Deep Learning dengan menggunakan 
Convolutional Neural Network (CNN). EfficientNet model digunakan untuk melatih 
dataset yang telah di pre-prosesing sebelumnya. Hasil dari penelitian tersebut 
didapatkan akurasi sebesar 79.8% yang dapat mengklasifikasi 5 level penyakit 
Diabetic Retinopathy. 

2. Dataset yang digunakan pada Jurnal
Data yang digunakan pada referensi tersebut merupakan data dari kaggle tentang Diabetic Retinopaty
https://www.kaggle.com/c/aptos2019-blindness-detection/data

3. Preprocessing Data pada Jurnal
Sebelum dimasukkan ke dalam model Deep Learning, perlu dilakukan pre-processing pada 
dataset citra input. Penulis menggunakan Contrast Limited Adapt ive Histogram Equalization
(CLAHE). CLAHE merupakan metode untuk meningkatkan untuk meningkatkan kontras pada citra. Berbeda dengan metode lain yang dapat 
meningkatkan kontrak citra lainnya, metode ini tidak akan meningkatkan kontras noise pada 
gambar. Hal ini dapat dilakukan dengan menentukan nilai clip limit (batas ambang) untuk 
dilakukan pemotongan dari bagian citra yang tidak diperlukan.

4. Model dan Hasil Akurasi
Sistem yang dibuat merupakan klasifikasi 5 kelas penyakit Diabetic Retinopathy dengan menggunakan CNN dengan model EfficientNet yang memiliki tingkat akurasi cukup tinggi dibandingkan dengan metode sebelumnya yaitu sebesar 79.8%. 

Hasil perbandingan model
![1](https://user-images.githubusercontent.com/92302616/143834212-25567652-6614-42c0-8e57-50e870c443f2.PNG)


# Overview Dataset


# Deskripsi Dataset
Diabetic Retinopathy merupakan suatu penyakit yang dapat menyebabkan kebutaan pada
penderitanya. Hal ini disebabkan karenanya terdapatnya sejumlah luka pada mata yang dapat
merusak retina pada mata. Pada tahap awal, terjadinya pelebaran pembuluh darah pada mata,
yang selanjutkan jika dibiarkan akan terbentuk pembuluh darah baru yang dapat menutup
retina mata yang berakhir pada kebutaan. Diabetic Retinopathy dibagi menjadi 2 kelas yaitu
non-proliferative Diabetic Retinopathy (NPDR), dan proliferative Diabetic Retinopathy (PDR).
NPDR adalah tahap awal pada Diabetic Retinopathy yang membentuk microaneurysms. PDR
adalah level akhir pada Diabetic Retinopathy yang berarti kerusakan pada mata sudah parah
yang dapat menyebabkan pecahnya pembuluh darah pada mata. Sedangkan berdasarkan tingkatannya, menurut para ahli Opthalmologist,
Diabetic Retinopathy diklasifikasikan kedalam 4 level kondisi: 1) Mild Non-proliferative, 2)
Moderate Non-proliferative, 3) Severe Non-proliferative, dan 4) Proliferative

# Teknik Deep Learning yang digunakan
1. Model dengan menggunakan algoritma ANN (Artificial Neural Network)
2. Model dengan menggunakan algoritma CNN (Convolutional Neural Network)

# Jurnal Referensi
Jurnal referensi pada projek ini berjudul Deep Learning untuk Klasifikasi Diabetic Retinopathy menggunakan Model EfficientNet
http://dx.doi.org/10.26760/elkomika.v8i3.693

# Cara Eksekusi Program
1. Download file .ipynb
2. Buka di Notebook anda atau google colabolatory

# Autors
1. Muhammad Marlianur (201810370311023)
2. Ernowo Gordon Unus (201810370311043)
