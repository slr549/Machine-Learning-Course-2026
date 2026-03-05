# Minggu 4: Classification & Logistic Regression 🩺

## Tujuan Pembelajaran
1. Memahami perbedaan mendasar antara **Regresi** (prediksi angka kontinu) dan **Klasifikasi** (prediksi kategori/kelas).
2. Memahami cara kerja fungsi *Sigmoid* dalam Logistic Regression.
3. Melakukan evaluasi model klasifikasi menggunakan **Confusion Matrix**.
4. Memahami metrik klasifikasi: *Accuracy, Precision, Recall,* dan *F1-Score*.

## Konsep Matematika: Fungsi Sigmoid
Berbeda dengan Regresi Linear yang menghasilkan garis lurus tak terbatas, Logistic Regression memeras hasil tebakan ke dalam rentang nilai antara 0 dan 1 (probabilitas). Ini dilakukan menggunakan fungsi **Sigmoid**:
$$\sigma(z) = \frac{1}{1 + e^{-z}}$$
Di mana $z = w_1x_1 + w_2x_2 + ... + b$.
Jika probabilitas $\ge 0.5$, model akan mengklasifikasikannya sebagai kelas 1 (Positif). Jika $< 0.5$, masuk ke kelas 0 (Negatif).

## Metrik Evaluasi Klasifikasi
Dalam klasifikasi, akurasi saja seringkali menipu (terutama jika data tidak seimbang). Kita butuh:
* **True Positive (TP) / True Negative (TN):** Tebakan benar.
* **False Positive (FP):** Ditebak positif, padahal aslinya negatif (Contoh: Didiagnosis kanker, padahal sehat - *Error Tipe 1*).
* **False Negative (FN):** Ditebak negatif, padahal aslinya positif (Contoh: Didiagnosis sehat, padahal kena kanker - *Error Tipe 2* / Sangat Fatal).
* **Precision:** Seberapa akurat tebakan positif kita?
* **Recall:** Seberapa banyak kelas positif yang berhasil kita temukan?
