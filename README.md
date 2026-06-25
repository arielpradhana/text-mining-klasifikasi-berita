# 📰 Text Mining: Klasifikasi Berita Indonesia

Proyek UAS Text Mining — Klasifikasi otomatis artikel berita berbahasa Indonesia dari Detik.com menggunakan algoritma machine learning.

## 📌 Deskripsi

Proyek ini membangun pipeline text mining end-to-end mulai dari crawling data, prapemrosesan teks, ekstraksi fitur TF-IDF, hingga pemodelan dan evaluasi menggunakan empat algoritma klasifikasi. Dataset terdiri dari 330 artikel berita dari tiga kategori: **Olahraga**, **Ekonomi**, dan **Hiburan**.

## 📂 Struktur Proyek

```
├── TextMining_Klasifikasi_Berita.ipynb    # Notebook utama (crawling hingga evaluasi)
├── berita.csv                             # Dataset mentah hasil crawling
├── berita_bersih.csv                      # Dataset setelah prapemrosesan
├── confusion_matrix_all.png               # Visualisasi confusion matrix
└── README.md
```

## ⚙️ Teknologi yang Digunakan

- Python 3.x
- BeautifulSoup4 — web crawling
- PySastrawi — stemming & stopword bahasa Indonesia
- Scikit-learn — TF-IDF, modeling, evaluasi
- Pandas, Matplotlib, Seaborn

## 🔄 Alur Pipeline

1. **Web Crawling** — Mengambil artikel dari sport.detik.com, finance.detik.com, hot.detik.com
2. **Prapemrosesan** — Cleaning, case folding, tokenisasi, stopword removal, stemming
3. **Ekstraksi Fitur** — TF-IDF (5.000 fitur, unigram + bigram)
4. **Pemodelan** — Naive Bayes, SVM Linear, Random Forest, Logistic Regression
5. **Evaluasi** — Akurasi, Presisi, Recall, F1-Score, Confusion Matrix

## 📊 Hasil Evaluasi

| Model               | Akurasi (%) | Presisi (%) | Recall (%) | F1-Score (%) |
|---------------------|-------------|-------------|------------|--------------|
| Naive Bayes         | 100.00      | 100.00      | 100.00     | 100.00       |
| SVM (Linear)        | 100.00      | 100.00      | 100.00     | 100.00       |
| Logistic Regression | 100.00      | 100.00      | 100.00     | 100.00       |
| Random Forest       | 98.48       | 98.55       | 98.48      | 98.48        |

## 🚀 Cara Menjalankan

1. Clone repo ini
```bash
git clone https://github.com/arielpradhana/text-mining-klasifikasi-berita.git
```

2. Install dependencies
```bash
pip install requests beautifulsoup4 pandas scikit-learn PySastrawi nltk matplotlib seaborn tqdm
```

3. Jalankan notebook `text_mining.ipynb` secara berurutan dari atas ke bawah

## 👤 Author

**Nama:** *(FIQRI ARIEL PRADHANA)*  
**NIM:** *(232410102085)*  
**Mata Kuliah:** Text Mining  
**Institusi:** *(UNIVERSITAS JEMBER)*
