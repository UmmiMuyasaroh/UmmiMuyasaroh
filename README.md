# 🛍️ Sentiment Analysis Komentar Aplikasi Shopee di Playstore

## 📌 Project Overview

Proyek ini bertujuan untuk mengklasifikasikan komentar pengguna aplikasi Shopee di Google Playstore ke dalam dua kategori sentimen: **positif (1)** dan **negatif (0)**. Dengan pendekatan NLP dan model Support Vector Machine (SVM), sistem ini dapat membantu mengidentifikasi persepsi publik terhadap aplikasi secara efisien dan otomatis.

Metode yang digunakan mencakup:
- **Web scraping** komentar pengguna dari Playstore
- **Preprocessing teks** menggunakan NLP (case folding, tokenisasi, stopword removal, stemming)
- **Ekstraksi fitur** menggunakan TF-IDF
- **Klasifikasi sentimen** menggunakan algoritma SVM

## 📂 Raw Dataset Link

Dataset dikumpulkan secara manual melalui scraping dari halaman ulasan aplikasi Shopee di Playstore.

📎 **(https://drive.google.com/file/d/1qd416TqdtMsoaWqbQJLU6zv2gXfAAApQ/view?usp=sharing))**  


---

## 📊 Insight & Findings

Berdasarkan hasil analisis dan evaluasi model:

| Metric     | Value |
|------------|-------|
| Precision  | 88%   |
| Recall     | 88%   |
| F1-Score   | 88%   |
| Accuracy   | 88%   |

- Model menunjukkan performa **yang seimbang antara presisi dan sensitivitas** terhadap kedua label (positif dan negatif).
- Komentar negatif sebagian besar mengandung keluhan terhadap performa aplikasi dan layanan pengiriman.
- Komentar positif didominasi oleh kata kunci seperti “murah”, “cepat”, dan “promo”.
- Hasil ini menunjukkan **Shopee memiliki citra positif**, tetapi ada masalah layanan yang tetap perlu diperbaiki.

---

## 🤖 AI Support Explanation

Model AI yang digunakan: **Support Vector Machine (SVM)**  
Framework: `scikit-learn`, `pandas`, `Sastrawi`, `matplotlib`

### 🔧 Tahapan Pengolahan AI:
1. **Preprocessing** teks dengan NLP:
   - Case folding
   - Stopword removal
   - Tokenization
   - Stemming
2. **Ekstraksi fitur** menggunakan **TF-IDF** untuk merepresentasikan kata sebagai vektor.
3. **Klasifikasi** menggunakan **SVM**, cocok untuk data teks berdimensi tinggi dan pemisahan linear/non-linear.
4. **Evaluasi model** dilakukan dengan `classification_report()` dan confusion matrix.

Model mencapai **akurasi 88%**, menunjukkan kemampuan yang cukup kuat untuk klasifikasi sentimen pada data komentar.

---
