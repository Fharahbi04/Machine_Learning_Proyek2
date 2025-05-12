# Machine Learning Submission
Proyek ini merupakan proyek yang sama seperti sebelumnya tetapi terdapat beberapa perubahan sedikit
## Data Yang di Peroleh
 - Data yang di pakai merupakan data OSN yang didapatkan dari kaggle.
 - Terdapat kolom kategori dan numerik


## Hasil Cluster
 - Cluster yang dihasilkan merupakan 3 cluster.
 - Cluster di kategorikan berdasar Provinsi,Tahun,Bidang,Kelas,Gender,Kab/Kota.
 - Hasil Silhoute Score = 0.70.
 - Melakukan Feature Selection dan mendapatkan perbandingan hasil silhoute score = 0.71.
### Visualisasi Cluster
```
<img width="559" alt="image" src="https://github.com/user-attachments/assets/0ee28533-139d-4dba-b3c5-a8837ac0c079" />
```
### Hasil Interpretasi Analisis Karakteristik Cluster 
```
####Cluster 0:
  - Rata-rata Tahun ke ikut sertaan: Tahun 2021
  - Rata-rata Bidang keikutsertaan (Geografi-Ipa): IPA
  - Analisis: Cluster ini mencakup provinsi yang belum terlalu maju dan masih perlu dukungan/perhatian lebih untuk masalah pendidikan,dan kemudian untuk cluster 0 ini bidang yang di ikuti mencakup tentang perhitungan alam seperti ipa dan matematika.
####Cluster 1:
  - Rata-rata Tahun ke ikut sertaan: 2020
  - Rata-rata Bidang keikutsertaan (Geografi-Ipa): IPS
  - Analisis: Cluster ini menunjukkan provinsi menengah tentang masalah pendidikan,dan bidang yang di ikuti mencakup tentang campuran antara hafalan dan perhitungan dimana ips dan matematika mendominasi.
####Cluster 2:
  - Rata-rata Tahun ke ikut sertaan: 2022
  - Rata-rata Bidang keikutsertaan (Geografi-Ipa): Matematika
  - Analisis: Cluster ini terdiri dari provinsi urban/maju seperti DKI Jakarta,Bali,Banten dan Sumbar,kemudian bidang yang di ikuti full tentang perhitungan yaitu matematika dan fisika.
```
## Klasifikasi
 - Klasifikasi berdasarkan cluster yang didapat.
 - Model Klasifikasi menggunakan Random Forest, dan SVM.
### Random Forest
 - Mendapatkan hasil = 1.0
### SVM
 - Mendapatkan hasil = 0.99
### Analisi Hasil Evaluasi
 - Berdasarkan hasil tunggin dan evaluasi yang diberikan,dapat dilihat bahwa setelah di tuning menggunakan randomized search menunjukkan bahwa angka recal di masing-masing target mengalami peningkatan yang artinya hasil tunning tersebut baik dan mengalami peningkatan.
 - Identifikasi kelemahan model, seperti:
   - Precision dan Recall pada model menggunakan algoritma SVM dibawah dari randomforest.
   - Kemungkinan besar model mengalami overvitting,dimana model belajar terlalu spesifik terhadap data latih.
   - Rekomendasi yang diberikan untuk kedepannya adalah,gunakan data uji yang berbeda,kurangi kompleksitas model,gunakan cross validation dan menambahkan regularization/pruning/ 

