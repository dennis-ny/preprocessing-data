# Sleep Health Data Preprocessing

## Dataset Overview
Dataset ini berisi data dummy tentang pola tidur dan faktor-faktor yang mempengaruhinya, termasuk konsumsi kafein, tekanan darah, dan kebiasaan penggunaan layar sebelum tidur. Data ini digunakan untuk analisis preprocessing dalam data mining.

## Struktur Dataset
Dataset memiliki 8 kolom dengan rincian sebagai berikut:

- **Jenis_Kelamin** → Laki-laki / Perempuan
- **Durasi_Tidur** → Jumlah jam tidur dalam semalam
- **Konsumsi_Kafein** → Berapa banyak kafein yang dikonsumsi dalam sehari (jumlah cangkir)
- **Tekanan_Darah** → Tekanan darah dalam satuan mmHg
- **Screen_Time** → Durasi penggunaan layar sebelum tidur (jam)
- **BMI** → Indeks Massa Tubuh
- **Kebiasaan_Bangun_Terlambat** → Ya / Tidak
- **Gangguan_Tidur** → Ya / Tidak

## Preprocessing Steps
Dalam preprocessing, dilakukan beberapa langkah utama:
1. **Handling Missing Values**
   - Mengisi nilai yang hilang pada kolom numerik dengan rata-rata.
   - Mengisi nilai yang hilang pada kolom kategorikal dengan modus.
2. **Encoding Categorical Data**
   - Menggunakan One-Hot Encoding untuk Jenis_Kelamin dan Kebiasaan_Bangun_Terlambat.
   - Menggunakan Label Encoding untuk Gangguan_Tidur.
3. **Feature Scaling**
   - Menggunakan StandardScaler untuk normalisasi data numerik.
4. **Splitting Dataset**
   - Memisahkan data menjadi training set dan testing set.

## Tools & Libraries
Preprocessing ini dilakukan menggunakan:
- Python
- NumPy (operasi numerik dan array)
- Pandas (manipulasi dan analisis data)
- Matplotlib (visualisasi data)

## Cara Menggunakan
1. Pastikan file dataset **data_kesehatan_tidur.csv** tersedia dalam direktori proyek.
2. Jalankan **Preprocessing_Data.ipynb** di Google Colab.
3. Hasil preprocessing akan digunakan untuk analisis lebih lanjut.

---
**Author:** *Dennis Noor Yahya*
