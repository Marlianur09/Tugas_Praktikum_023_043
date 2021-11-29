# Tugas_Praktikum_023_043
- Autors
1. Muhammad Marlianur (201810370311023)
2. Ernowo Gordon Unus (201810370311043)
# Klasifikasi Diabetic Retinopaty Menggunakan CNN

# Overview Jurnal Referensi
1. Jurnal Referensi

- Jurnal referensi pada projek ini berjudul Deep Learning untuk Klasifikasi Diabetic Retinopathy menggunakan Model EfficientNet
- Link Jurnal : http://dx.doi.org/10.26760/elkomika.v8i3.693
- Diabetic Retinopathy merupakan penyakit yang dapat mengakibatkan kebutaan mata yang disebabkan oleh adanya komplikasi penyakit diabetes melitus. Oleh karena itu mendeteksi secara dini sangat diperlukan untuk mencegah bertambah parahnya penyakit tersebut. Penelitian ini merancang sebuah sistem yang dapat mendeteksi Diabetic Retinopathy berbasis Deep Learning dengan menggunakan Convolutional Neural Network (CNN). EfficientNet model digunakan untuk melatih dataset yang telah di pre-prosesing sebelumnya. Hasil dari penelitian tersebut didapatkan akurasi sebesar 79.8% yang dapat mengklasifikasi 5 level penyakit Diabetic Retinopathy. 

2. Dataset yang digunakan pada Jurnal

- Data yang digunakan pada referensi tersebut merupakan data dari kaggle tentang Diabetic Retinopaty
https://www.kaggle.com/c/aptos2019-blindness-detection/data

3. Preprocessing Data pada Jurnal

- Sebelum dimasukkan ke dalam model Deep Learning, perlu dilakukan pre-processing pada dataset citra input. Penulis menggunakan Contrast Limited Adapt ive Histogram Equalization (CLAHE). CLAHE merupakan metode untuk meningkatkan untuk meningkatkan kontras pada citra. Berbeda dengan metode lain yang dapat meningkatkan kontrak citra lainnya, metode ini tidak akan meningkatkan kontras noise pada gambar. Hal ini dapat dilakukan dengan menentukan nilai clip limit (batas ambang) untuk dilakukan pemotongan dari bagian citra yang tidak diperlukan.

4. Model dan Hasil Akurasi

- Sistem yang dibuat merupakan klasifikasi 5 kelas penyakit Diabetic Retinopathy dengan menggunakan CNN dengan model EfficientNet yang memiliki tingkat akurasi cukup tinggi dibandingkan dengan metode sebelumnya yaitu sebesar 79.8%. 

- Hasil perbandingan model

![1](https://user-images.githubusercontent.com/92302616/143834212-25567652-6614-42c0-8e57-50e870c443f2.PNG)


# Overview Dataset

1. Link Dataset

- https://www.kaggle.com/c/aptos2019-blindness-detection/data

2. Tentang Dataset
- Judul dataset adalah APTOS 2019 Blindness Detection (Detect diabetic retinopathy to stop blindness before it's too late)
- Diabetic Retinopathy merupakan suatu penyakit yang dapat menyebabkan kebutaan pada penderitanya. Hal ini disebabkan karenanya terdapatnya sejumlah luka pada mata yang dapat merusak retina pada mata. Pada tahap awal, terjadinya pelebaran pembuluh darah pada mata, yang selanjutkan jika dibiarkan akan terbentuk pembuluh darah baru yang dapat menutup retina mata yang berakhir pada kebutaan. Diabetic Retinopathy dibagi menjadi 2 kelas yaitu non-proliferative Diabetic Retinopathy (NPDR), dan proliferative Diabetic Retinopathy (PDR). NPDR adalah tahap awal pada Diabetic Retinopathy yang membentuk microaneurysms. PDR adalah level akhir pada Diabetic Retinopathy yang berarti kerusakan pada mata sudah parah yang dapat menyebabkan pecahnya pembuluh darah pada mata. Sedangkan berdasarkan tingkatannya, menurut para ahli Opthalmologist, Diabetic Retinopathy diklasifikasikan kedalam 4 level kondisi: 1) Mild Non-proliferative, 2) Moderate Non-proliferative, 3) Severe Non-proliferative, dan 4) Proliferative
- Jumlah gambar yaitu 5590 gambar
- Hanya memilki satu kelas
- Dataset dibagi menjadi 2 yaitu Data test_images dan Data train_images
- Data test_images berisi 1928 gambar dengan ukuran 2 GB
- Data train_images berisi 3662 gambar dengan ukuran 8 GB

# Teknik Deep Learning yang digunakan
1. Model dengan menggunakan algoritma ANN (Artificial Neural Network)
2. Model dengan menggunakan algoritma CNN (Convolutional Neural Network)

# Cara Eksekusi Program
1. Download file .ipynb
2. Buka di Notebook anda atau google colabolatory

# Preprocessing Dataset
- grayscale=False
- color_mode='rgb'
- target_size=(60,60)
- horizontal_flip=True
- vertical_flip=True
- rotation_range=20
- zoom_range=0.2
- width_shift_range=0.2
- height_shift_range=0.2
- shear_range=0.1
- fill_mode="nearest

# Model yang digunakan Dataset
Model yang digunakan adalah CNN (Convolutional Neural Network), untuk lebih jelasnya lihat hasil modul

# Hasil Modul 1
- Pada modul 1 tugas yang diberikan masih tentang pembuatan GitHub untuk praktikum pembelajaran mesin, belum berkaitan dengan pengolahan dataset
# Hasil Modul 2
1. Melakukan proses preprocessing dataset
- 
2. Melakukan training beberapa skema model menggunakan model CNN sederhana buatan sendiri (minimal 2 model) tidak diperbolehkan menggunakan transfer learning
- Hasil Menggunakan model
- ![model 1 acc](https://user-images.githubusercontent.com/92302616/143843189-b7a1da29-fce4-46cf-8957-f98e42ec389a.PNG)
- ![model 2 acc](https://user-images.githubusercontent.com/92302616/143843186-cfa40b2a-aabd-459f-92e5-ef11225aa7e6.PNG)







- Hasil acc dan loss Model 1



![1](https://user-images.githubusercontent.com/92302616/143843951-db2b8b3b-75d4-40e2-99c4-658b7d27dee6.png)
![2](https://user-images.githubusercontent.com/92302616/143843969-f6192d96-2f73-4623-8074-a4e2941d49f7.png)





- Hasil acc dan loss Model 2




![3](https://user-images.githubusercontent.com/92302616/143844264-fc89003c-839a-4118-946c-c714b61509bc.png)
![4](https://user-images.githubusercontent.com/92302616/143844275-4a3f7318-8e22-402e-8068-3aa3f3ae2809.png)



3. Menyimpan model yang telah di training kedalam file .h5


# Hasil Modul 3
# Hasil Modul 4
# Hasil Modul 5
# Hasil Modul 6

