# Minggu 3: Linear Regression & Regularization (L1/L2) 🏠

## Tujuan Pembelajaran
1. Memahami konsep dasar Multiple Linear Regression.
2. Mencegah *Overfitting* menggunakan teknik Regularisasi (Ridge & Lasso).
3. Mengimplementasikan model menggunakan **Scikit-Learn**.
4. Melacak performa berbagai model menggunakan **W&B**.

## 1. Metrik Evaluasi
Untuk mengetahui seberapa akurat prediksi kita, kita menggunakan:
1. **Mean Absolute Error (MAE):** Rata-rata selisih absolut antara prediksi dan nilai asli.
2. **Mean Squared Error (MSE):** Rata-rata selisih kuadrat (memberikan penalti lebih besar pada error besar).
3. **Root Mean Squared Error (RMSE):** Akar dari MSE agar satuannya kembali sama dengan unit target.

## 2. Multiple Linear Regression
Regresi Linear mencoba mencari bobot ($w$) terbaik untuk setiap fitur agar menghasilkan prediksi ($y$) yang paling akurat. Persamaannya:
$$y = w_1x_1 + w_2x_2 + ... + w_nx_n + b$$

## 3. Mengapa Butuh Regularisasi?
Saat kita memiliki terlalu banyak fitur, model bisa menjadi terlalu kompleks dan menghafal data *training* (Overfitting). Regularisasi adalah teknik menambahkan "hukuman" (penalty) pada bobot ($w$) yang terlalu besar.

* **L2 Regularization (Ridge):** Menciutkan bobot agar mendekati nol, tapi tidak sampai nol. Sangat baik untuk mencegah multikolinearitas.
  $$Cost = MSE + \alpha \sum_{i=1}^{n} w_i^2$$

* **L1 Regularization (Lasso):** Bisa menciutkan bobot fitur yang tidak penting hingga **tepat menjadi nol**. Ini sekaligus berfungsi sebagai *Feature Selection* otomatis.
  $$Cost = MSE + \alpha \sum_{i=1}^{n} |w_i|$$


