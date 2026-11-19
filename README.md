# PROYEK AKHIR PEMBELAJARAN MESIN DASAR
## KELOMPOK 1

# Prediksi Viralitas Konten TikTok Menggunakan Machine Learning

## Anggota Kelompok

| No. | Nama | NIM |
|:---:|---|:---:|
| 1 | Yanaka Sofia Pardede | 24031554065 |
| 2 | Ayu Wulan Anggraeni Putri | 24031554177 |
| 3 | Annisa Ramadhani | 24031554206 |

**Kelas:** 2024B

---

## Deskripsi Proyek

Proyek ini merupakan proyek akhir mata kuliah **Pembelajaran Mesin Dasar** yang bertujuan untuk memprediksi viralitas konten TikTok berdasarkan data *engagement* pengguna menggunakan metode *Machine Learning*.

Dataset yang digunakan adalah **TikTok 2025 Dataset** yang diperoleh dari Kaggle. Dataset ini terdiri dari 7.225 data konten TikTok dengan beberapa atribut utama, yaitu *likes, comments, shares,* dan *plays*.

Penelitian dilakukan melalui beberapa tahapan, mulai dari pemahaman dan preprocessing data, penanganan ketidakseimbangan kelas menggunakan SMOTE, seleksi fitur menggunakan SelectKBest, hingga pembangunan dan evaluasi model klasifikasi menggunakan Support Vector Machine (SVM) dan Multi-Layer Perceptron (MLP).

Melalui proyek ini, dilakukan perbandingan performa kedua algoritma untuk mengetahui model yang memberikan hasil klasifikasi terbaik dalam memprediksi konten viral dan tidak viral.

## Dataset

Dataset yang digunakan dalam penelitian ini adalah:

- **Nama Dataset:** TikTok 2025 Dataset
- **Sumber:** Kaggle
- **Jumlah Data:** 7.225 konten TikTok
- **Link Dataset:** [TikTok 2025 Dataset - Kaggle](https://www.kaggle.com/datasets/haziqhalifi/tiktok-2025-dataset)

### Fitur yang Digunakan

| Fitur | Deskripsi |
|---|---|
| Likes | Jumlah suka pada video |
| Comments | Jumlah komentar pada video |
| Shares | Jumlah video dibagikan |
| Plays | Jumlah tayangan video |

## Tahapan Penelitian

Penelitian ini dilakukan melalui beberapa tahapan sebagai berikut:

1. **Dataset Collection:** Mengumpulkan dataset TikTok 2025 dari Kaggle.
2. **Data Understanding:** Memahami struktur, karakteristik, dan atribut dataset.
3. **Data Preprocessing:** Melakukan persiapan dan pengolahan data sebelum pemodelan.
4. **Data Balancing:** Menangani ketidakseimbangan kelas menggunakan SMOTE.
5. **Exploratory Data Analysis (EDA):** Mengeksplorasi karakteristik dan pola data melalui analisis serta visualisasi.
6. **Feature Selection:** Memilih fitur yang relevan menggunakan SelectKBest.
7. **Data Splitting:** Membagi dataset menjadi data latih dan data uji.
8. **Model Development:** Membangun model klasifikasi menggunakan SVM dan MLP.
9. **Model Evaluation:** Mengevaluasi performa model menggunakan metrik klasifikasi.
10. **Result Analysis:** Menganalisis dan membandingkan hasil prediksi dari kedua model.

## Metode yang Digunakan

### 1. Feature Selection

Metode seleksi fitur yang digunakan adalah **SelectKBest dengan ANOVA F-Test** untuk mengidentifikasi fitur yang memiliki hubungan paling relevan dengan target klasifikasi.

### 2. Data Balancing

Penanganan ketidakseimbangan kelas dilakukan menggunakan **SMOTE (Synthetic Minority Oversampling Technique)**, yaitu teknik oversampling untuk membantu menyeimbangkan distribusi kelas pada data pelatihan.

### 3. Machine Learning Models

Dua algoritma klasifikasi yang digunakan dalam penelitian ini adalah:

- **Support Vector Machine (SVM):** Algoritma klasifikasi yang mencari hyperplane terbaik untuk memisahkan kelas data.
- **Multi-Layer Perceptron (MLP):** Model jaringan saraf tiruan yang menggunakan beberapa lapisan neuron untuk mempelajari pola dalam data.

## Hasil Feature Selection

Berdasarkan proses seleksi fitur menggunakan SelectKBest dengan ANOVA F-Test, diperoleh hasil sebagai berikut:

| Ranking | Feature | Score |
|:---:|---|---:|
| 1 | Plays | 1947.20 |
| 2 | Likes | 1580.23 |
| 3 | Shares | 738.03 |
| 4 | Comments | 317.73 |

Hasil seleksi menunjukkan bahwa fitur **Plays** memperoleh skor tertinggi, sehingga menjadi fitur dengan nilai statistik paling kuat dalam proses seleksi fitur berdasarkan ANOVA F-Test.

## Hasil Evaluasi Model

Evaluasi dilakukan untuk membandingkan performa algoritma SVM dan MLP berdasarkan empat metrik, yaitu Accuracy, Precision, Recall, dan F1-Score.

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| SVM | 97.92% | 92.61% | 100.00% | 96.16% |
| MLP | 100.00% | 100.00% | 100.00% | 100.00% |

Berdasarkan hasil evaluasi, model **Multi-Layer Perceptron (MLP)** memberikan performa terbaik pada dataset yang digunakan dengan nilai Accuracy, Precision, Recall, dan F1-Score masing-masing sebesar 100%.

Sementara itu, model Support Vector Machine (SVM) memperoleh Accuracy sebesar 97,92% dengan F1-Score sebesar 96,16%.

## Kesimpulan

Berdasarkan penelitian yang telah dilakukan, data *engagement* TikTok dapat dimanfaatkan untuk melakukan klasifikasi konten viral dan tidak viral menggunakan pendekatan *Machine Learning*.

Keempat fitur yang digunakan, yaitu *plays, likes, shares,* dan *comments*, memberikan informasi yang relevan dalam proses klasifikasi. Berdasarkan hasil seleksi fitur, *plays* memperoleh skor ANOVA F-Test tertinggi dibandingkan fitur lainnya.

Dari dua algoritma yang diuji, Multi-Layer Perceptron (MLP) menghasilkan performa terbaik dengan nilai Accuracy, Precision, Recall, dan F1-Score sebesar 100%. Sementara itu, Support Vector Machine (SVM) menghasilkan Accuracy sebesar 97,92%.

Dengan demikian, MLP menjadi model dengan performa terbaik pada eksperimen ini berdasarkan hasil evaluasi yang diperoleh.
