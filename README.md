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



![6](https://user-images.githubusercontent.com/92302616/143853650-d932bf4d-0060-4dc5-b4d6-3858dc8304f2.PNG)


# Hasil Modul 3
1. Melakukan proses preprocessing dataset dengan ketentuan:
- augmentasi data menggunakan ImageDataGenerator
- splitting dataset menjadi (75% train, 14% validation, 1% test)
- Jawaban : Berdasarkan pembahasan bersama aslab, Dataset yang kami gunakan telah di split dari kaggle sehingga tidak perlu di split lagi.
2. Melakukan training beberapa skema model menggunakan model CNN sederhana buatan sendiri (minimal 2 model) tidak diperbolehkan menggunakan transfer learning
- Menerapkan proses Convolution
- Menerapkan proses Pooling
- Menerapkan Dropout
- Menerpakan BatchNormalization
- Model dengan beberapa variasi learning rate
- Minimal 100 epoch per model



- Hasil dari tugas di atas untuk model 1 dan model 2:

![1](https://user-images.githubusercontent.com/92302616/143858517-ed25d88f-808b-4564-95af-8d4b2601dec3.PNG)
![2](https://user-images.githubusercontent.com/92302616/143858528-fb32e1e5-be18-4bed-a9df-f55d9e9a485b.PNG)





- Hasil acc dan loss model 1


![11](https://user-images.githubusercontent.com/92302616/143859226-05634242-dbbb-4d3c-80aa-7c44680320f0.png)
![12](https://user-images.githubusercontent.com/92302616/143859242-2d141467-b3d4-44bf-a381-e28673466c0d.png)








- Hasil acc dan loss model 2


![21](https://user-images.githubusercontent.com/92302616/143859347-dbec6c44-f517-461f-9c6d-0c25a2bc1d70.png)
![22](https://user-images.githubusercontent.com/92302616/143859361-a5e7e517-be19-44ab-8659-d63b1c87505e.png)


# Hasil Modul 4
1. Melakukan proses preprocessing dataset dengan ketentuan:
- augmentasi data menggunakan ImageDataGenerator
- balancing dataset menggunakan teknik oversampling / downsampling
- splitting dataset menjadi (75% train, 14% validation, 1% test)
2. Melakukan training beberapa skema model menggunakan model CNN sederhana buatan sendiri (minimal 2 model) tidak diperbolehkan menggunakan transfer learning
- Menerapkan proses Convolution
- Menerapkan proses Pooling
- Menerapkan Dropout
- Menerpakan BatchNormalization
- Menerapkan learning rate scheduller
- Menggunakan hyperparameter tuning
- Minimal 100 epoch per model
# Hasil
- Menggunakan Hyper Parameter Tuning


![Capture](https://user-images.githubusercontent.com/92302616/144702865-d2d961da-4ff5-4e44-b2c4-8102770ee0d3.PNG)


- Epoch menggunakan HParam


![2](https://user-images.githubusercontent.com/92302616/144702847-a5f19b66-ce14-480f-a8c3-d83b4afd6cae.PNG)


- Akurasi paling tinggi hasil dari optimizer adam


![3](https://user-images.githubusercontent.com/92302616/144702849-2476b072-e88f-42cf-a5e7-45155efa14a9.PNG)


# Hasil Modul 5
- Melakukan proses preprocessing dataset dengan ketentuan: augmentasi data menggunakan ImageDataGenerator dan salah satu augmentasi opsional lain seperti (random noise, clahe, usuyama, blur, atau yang lainnya), balancing dataset menggunakan teknik oversampling / downsampling, splitting dataset menjadi (75% train, 14% validation, 1% test).
- Melakukan training beberapa skema model menggunakan pretrained model (minimal 2 model) dengan 100 epoch per model
- Menyimpan model yang telah di training kedalam file .tflite Lihat disini
# Hasil
- hasil Model-model yang digunakan

- Summary model pertama





![2](https://user-images.githubusercontent.com/92302616/146187885-d69e9a51-06bc-4740-91de-a29381e37529.PNG)




- Hasil akurasi Model pertama




![m12](https://user-images.githubusercontent.com/92302616/146187892-e1b40aa8-c2f5-45ca-a2a5-7c366e66c646.png)
![m1](https://user-images.githubusercontent.com/92302616/146187893-ef6f4e51-3701-41f3-b850-9a423134fdd1.png)




- Model kedua menggunakan Resnet152V2



![1](https://user-images.githubusercontent.com/92302616/146188326-3609d8f3-249e-48ce-9cda-e73eefc78311.PNG)





- Summary Model kedua




![3](https://user-images.githubusercontent.com/92302616/146188401-3166a98c-f5f7-4ab7-95f4-7060fbb10208.PNG)




- Hasil Akurasi Training Model ResNet152V2 yang terkendala atau sering stop di epoch ke 5



![hasil m2](https://user-images.githubusercontent.com/92302616/146188586-0a8d9b4d-9c8d-489d-ae9d-b22a24cf3b45.PNG)




- Hasil klasifikasi 5 level Diabetic Retinopaty



![m21](https://user-images.githubusercontent.com/92302616/146188719-ec230982-0256-44fa-90d5-50abf184a1df.png)
![m22](https://user-images.githubusercontent.com/92302616/146188724-da86784f-9ea9-4902-923f-dca1421314d9.PNG)

# Hasil Modul 6
1. Pre-requirement
- Membuat virtual environment python atau anaconda python
- Menjalankan virtual environment dan menginstall seluruh package yang digunakan dalam kegiatan ini pada virtual environment.
- Membuat file requirement.txt yang berisi seluruh paket package digunakan dalam kegiatan bagian B.
- Deployment menggunakan flask micro framework dari python
- Project berbasis python file berekstensi .py bukan file notebook .ipynb

2. Kriteria wajib untuk deploy model
- Menggunakan model yang telah dilatih dan disimpan dalam format .h5,.json dan .tflite pada kegiatan kelompok di modul - modul sebelumnya.
- Memiliki fitur upload data untuk diprediksi oleh model
- Memiliki menu pilih model untuk memilih model yang ingin digunakan untuk memprediksi gambar.
- Memiliki fitur komparasi model (fitur untuk membandingankan kinerja dari beberapa model dalam memprediksi data baru)
- Memiliki fitur pilih gambar yang terdiri dari 25 gambar acak untuk diprediksi. Masing-masing kelas dari dataset anda harus terwakili oleh minimal 1 buah gambar.
- Menampilkan hasil akurasi prediksi, lama waktu prediksi, input gambar yang dipresiksi dan label gambar yang diprediksi.
- Menyimpan seluruh progress dan hasil pengerjaan modul dalam repository github.

# Hasil
- Link Program : https://drive.google.com/drive/folders/1ggxifsJxIpE4vFWV6-_Si0klqWoT_e8M?usp=sharing

- Hasil deploy program
- Tampilan depan




![photo_2021-12-28_15-21-49](https://user-images.githubusercontent.com/92302616/147545463-be7121d6-dca6-461a-ae3d-20825d7321c9.jpg)
![photo_2021-12-28_15-21-49 (2)](https://user-images.githubusercontent.com/92302616/147545469-039d9bf3-1809-495a-8f12-c098b21bdfbb.jpg)




- Tampilan setelah penginputan gambar





![photo_2021-12-28_15-21-20](https://user-images.githubusercontent.com/92302616/147545689-8516a725-e21e-42ba-bee5-3a66fd0c2be0.jpg)
![photo_2021-12-28_15-21-20 (2)](https://user-images.githubusercontent.com/92302616/147545699-3a491585-05cc-44fd-be69-9fdc44be9428.jpg)
![photo_2021-12-28_15-21-21](https://user-images.githubusercontent.com/92302616/147545712-e6e941b9-80b9-4e39-8507-00b3664410b4.jpg)
![photo_2021-12-28_15-21-19](https://user-images.githubusercontent.com/92302616/147545720-dfec27a7-6ecf-467c-9b2b-408dfd1e71e5.jpg)
![photo_2021-12-28_15-21-19 (2)](https://user-images.githubusercontent.com/92302616/147545741-10122d7c-c337-4e67-81cb-8a694367e95b.jpg)


- Catatan :
1. Pada uji coba deploy didapatkan hasil bahwa dari tiga skenario model terlihat Model CNN dan Resnet50 memberikan akurasi tertinggi pada kelas NO DR masing-masing 100% dan 71%. Sedangkan pada model MobileNet memiliki akurasi tertinggi sekitar 99% pada kelas Moderate.
2. Deploy ini memiliki kekurangan pada tampilan hasil gambar. Gambar yang ditampilkan saat result masih sering gagal muncul, tetapi pada saat uji coba pertama hal tersebut masih bisa di atasi.
