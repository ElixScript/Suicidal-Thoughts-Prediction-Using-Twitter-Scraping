# Klasifikasi Suicidal Thoughts dengan Machine Learning

Repository ini berisi implementasi proyek *Penggunaan Model Machine Learning dalam Pembentukan Model Klasifikasi Suicidal Thoughts Menggunakan Data Twitter/X*. Proyek ini bertujuan untuk mendeteksi indikasi pemikiran bunuh diri berdasarkan data dari jejaring sosial **Twitter/X** menggunakan berbagai teknik *Natural Language Processing (NLP)* dan model *Machine Learning*.

## Latar Belakang

Setiap tahun, 703,000 orang di dunia mengakhiri hidupnya, dengan bunuh diri menjadi penyebab kematian keempat pada usia 15-29 tahun. Di Indonesia sendiri, terdapat 6,544 kasus kematian akibat bunuh diri pada tahun 2019. Dengan memanfaatkan data dari Twitter/X, proyek ini bertujuan untuk mendeteksi dini pemikiran bunuh diri sehingga dapat diarahkan kepada layanan bantuan seperti hotline atau psikolog.

## Metodologi

### 1. Data Collection
Dataset dikumpulkan dengan melakukan *scraping* pada platform Twitter/X menggunakan Python. Kata kunci seperti "capek hidup", "depresi", dan "nyerah" digunakan untuk mendapatkan data sebanyak 3000 *tweets* dalam format CSV.

### 2. Data Preprocessing
Tahapan pembersihan dan transformasi data mencakup:
- **Data Cleaning**: Menghapus elemen-elemen tidak relevan seperti *mention*, hashtag, dan URL.
- **Normalisasi**: Mengubah kata-kata tidak baku menjadi baku.
- **Spell Correction**: Memperbaiki kesalahan ejaan.
- **Stopword Deletion**: Menghapus kata-kata yang tidak memiliki makna signifikan.
- **Tokenization & Lemmatization**: Membagi teks menjadi unit-unit kecil dan mengubahnya menjadi bentuk dasar.
- **Labeling**: Menggunakan model *DistilBERT* untuk memberikan label (*neutral*, *positive*, *negative*).

### 3. Fine-Tuning dan Modelling
Model yang digunakan meliputi:
- **Random Forest**
- **Support Vector Machine (SVM)**
- **IndoBERT**

### 4. Validasi dan Evaluasi
Model diuji untuk mendapatkan akurasi terbaik dengan hasil sebagai berikut:
- SVM: 84.8%
- Random Forest: 84%
- IndoBERT: 87%

## Implementasi
Proses dan eksperimen dapat diakses melalui Google Colab:
[Google Colab Link](https://colab.research.google.com/drive/1xgsFLlj5MxSutfGUnPW6Q2izh-MRwj4E?usp=sharing)

## Hasil Analisis
Model **IndoBERT** memberikan performa terbaik dengan akurasi sebesar 87%, menunjukkan kemampuan unggul dalam memahami konteks teks yang kompleks.

## Kelebihan
- Fokus pada isu kesehatan mental pengguna media sosial.
- Data yang digunakan bersifat original.
- Menggunakan *state-of-the-art* model NLP seperti IndoBERT.

## Kekurangan
- Dataset hanya berisi 3000 *tweets*, menyebabkan model cenderung bias terhadap data negatif.
- Belum ada implementasi dalam bentuk *web application*.

## Kesimpulan
Proyek ini menunjukkan bahwa metode IndoBERT efektif dalam mendeteksi kecenderungan bunuh diri pada *tweets*. Dengan penambahan data dan pengurangan ketidakseimbangan dataset, akurasi model dapat ditingkatkan lebih lanjut.

---

