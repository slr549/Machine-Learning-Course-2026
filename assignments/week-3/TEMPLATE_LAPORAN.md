# 📑 Laporan Praktikum Minggu 3: Linear Regression & Regularization

**Informasi Mahasiswa:**

* **Nama:** [Isi Nama Anda]
* **NIM:** [Isi NIM Anda]
* **Link W&B Project:** [Paste Link Dashboard W&B Anda]
* **Link Pull Request GitHub:** [Paste Link PR Tugas Anda]

---

## 1. Pendahuluan

Jelaskan secara singkat perbedaan utama antara Regresi Linear Standar, Ridge Regression (L2), dan Lasso Regression (L1). Mengapa kita membutuhkan teknik regularisasi saat melatih model Machine Learning?

> **Jawaban:** (Tulis penjelasan Anda di sini)

---

## 2. Pemahaman Dataset

Pada praktikum ini, kita menggunakan dataset **California Housing**.

* Apa variabel target () yang ingin kita prediksi?
* Mengapa kita perlu membuang kolom teks (`ocean_proximity`) dan baris yang kosong (`dropna`) sebelum memasukkannya ke dalam model Regresi Linear Scikit-Learn?

> **Jawaban:** (Tulis penjelasan Anda di sini)

---

## 3. Hasil Baseline Model (Tanpa Hukuman)

Berdasarkan eksperimen pertama menggunakan `LinearRegression` biasa (tanpa regularisasi):

* **RMSE:** [Isi nilai RMSE]
* ** Score:** [Isi nilai ]
* **Interpretasi:** Apa arti dari nilai RMSE tersebut dalam konteks harga rumah di California?

---

## 4. Eksperimen Regularisasi "The Power of Alpha" (Tugas Inti)

Isi tabel di bawah ini berdasarkan hasil eksperimen Anda saat mengubah nilai parameter `alpha` pada model Ridge dan Lasso.

| Model | Alpha () | RMSE |  Score | Catatan Visualisasi Bobot (Blok 5) |
| --- | --- | --- | --- | --- |
| **Ridge** | 0.1 | ... | ... | (Misal: Bobot masih mirip dengan linear) |
| **Ridge** | 100 | ... | ... | ... |
| **Ridge** | 1000 | ... | ... | (Misal: Semua bobot mulai menciut mendekati 0) |
| **Lasso** | 0.1 | ... | ... | ... |
| **Lasso** | 100 | ... | ... | ... |
| **Lasso** | 1000 | ... | ... | (Misal: Beberapa fitur benar-benar menjadi 0) |

**Analisis Hasil Eksperimen:**

1. Apa yang terjadi pada nilai RMSE jika nilai `alpha` dibuat terlalu besar (misal 1000)? Apakah model menjadi lebih pintar atau justru mengalami *Underfitting*?
2. Berdasarkan grafik visualisasi bobot, algoritma mana (Ridge atau Lasso) yang secara agresif membuang fitur hingga nilai bobotnya tepat nol?

> **Jawaban:** (Tulis penjelasan Anda di sini)

---

## 5. Dokumentasi Weights & Biases (W&B)

Lampirkan *screenshot* dari *dashboard* W&B Anda. Karena Anda melakukan banyak eksperimen dengan berbagai nilai `alpha`, panel W&B Anda sekarang seharusnya menampilkan banyak titik eksperimen untuk metrik RMSE dan .

> **[Tempel Screenshot Dashboard W&B Anda di Sini]**

---

## 6. Kesimpulan & Refleksi

* Dari seluruh eksperimen di atas, model dengan pengaturan parameter apa yang menghasilkan performa terbaik (RMSE terendah dan  tertinggi)?
* Apa tantangan terbesar Anda saat mengerjakan praktikum minggu ini?

---

### Instruksi Pengumpulan:

1. Isi template ini dengan lengkap dan teliti.
2. Simpan sebagai file **PDF** atau **Markdown** (`.md`).
3. Kumpulkan tugas Anda dengan membuat folder `NIM_NAMA` di dalam folder `assignments/week-3/` pada *fork* repositori Anda.
4. Kirimkan pekerjaan Anda melalui **Pull Request** ke repositori utama dosen, dan pastikan judul PR sesuai format. Dosen akan melakukan proses **Squash and merge** untuk menjaga kerapian riwayat komit.

---
