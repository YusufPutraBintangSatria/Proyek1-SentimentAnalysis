# Proyek 1 – Sentiment Analysis App

## Deskripsi Singkat
Proyek ini bertujuan membangun model analisis sentimen untuk mengklasifikasikan ulasan film sebagai **positif** atau **negatif**. Model dikembangkan melalui beberapa tahapan: pengumpulan data, pra-pemrosesan, pemodelan, evaluasi, dan visualisasi.

## Dataset
- **Sumber:** Kaggle – [IMDB Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)
- **Jumlah Data:** 50.000 ulasan (25.000 positif, 25.000 negatif)

## Cleaning & Preprocessing
Langkah pra-pemrosesan:
1. Penanganan missing values → tidak ada nilai hilang.
2. Normalisasi teks → lowercase + hapus karakter non-alfanumerik.
3. Tokenisasi → memecah teks menjadi kata.
4. Stopword removal → menghapus kata umum untuk fokus kata penting.

## Model & Evaluasi
- **Model:** Pipeline `CountVectorizer` + `Multinomial Naive Bayes`
- **Data Split:** 80% training, 20% testing
- **Metrik Kinerja:**
  - Accuracy: 86.18%
  - F1-Score Negatif: 0.86
  - F1-Score Positif: 0.86
- **Confusion Matrix:**
[[4361 600]
[ 782 4257]]


## Hasil Visualisasi
- **Distribusi Sentimen:** Bar plot jumlah ulasan positif vs negatif  
  ![Distribusi Sentimen](Proyek1-SentimentAnalysis/Proyek_1_–_Sentiment_Analysis
/Visualisasi/Visualisasi_Distribution_of_Sentiments.png)
- **Word Cloud:** Kata-kata paling sering muncul setelah preprocessing  
  ![Word Cloud](Proyek1-SentimentAnalysis/Proyek_1_–_Sentiment_Analysis
/Visualisasi/Visualisasi_Word_Cloud_of_Reviews.png)

## Cara Menjalankan
1. Buka `notebook.ipynb` di Google Colab atau Jupyter Notebook.
2. Jalankan semua cell.
3. Model siap digunakan untuk prediksi review baru.


