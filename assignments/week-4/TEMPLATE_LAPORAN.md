# 📑 Laporan Praktikum Minggu 4: Logistic Regression & Confusion Matrix

**Informasi Mahasiswa:**

* **Nama:** [Isi Nama Anda]
* **NIM:** [Isi NIM Anda]
* **Link W&B Project:** [Paste Link Dashboard W&B Anda]
* **Link Pull Request GitHub:** [Paste Link PR Tugas Anda]

---

## 1. Pemahaman Konsep Dasar

Jelaskan dengan bahasa Anda sendiri:

1. Apa perbedaan utama antara masalah **Regresi** (Minggu 3) dan masalah **Klasifikasi** (Minggu 4)?
2. Bagaimana fungsi **Sigmoid** bekerja mengubah angka matematis (dari $-\infty$ hingga $\infty$) menjadi sebuah keputusan kelas (0 atau 1)?

> **Jawaban:** (Tulis penjelasan Anda di sini)

---

## 2. Hasil Evaluasi Metrik (Dataset Titanic)

Berdasarkan model `LogisticRegression` yang telah Anda latih untuk memprediksi keselamatan penumpang Titanic, tuliskan hasil metrik pada data *Testing*:

* **Accuracy  :** [Isi nilai akurasi]
* **Precision :** [Isi nilai precision]
* **Recall    :** [Isi nilai recall]
* **F1-Score  :** [Isi nilai f1-score]

---

## 3. Bedah Kritis: Confusion Matrix & Bahaya Kematian

*Machine Learning bukan sekadar angka akurasi. Sebuah model dengan akurasi 95% bisa saja sangat berbahaya jika digunakan di dunia nyata.*

Perhatikan *Confusion Matrix* dari prediksi Titanic Anda. Ingat bahwa:

* **Kelas 0:** Meninggal
* **Kelas 1:** Selamat

**A. Petakan angka dari grafik matriks Anda ke dalam 4 kuadran berikut:**

1. **True Negative (TN):** Asli Meninggal, ditebak Meninggal = [Isi jumlah orang]
2. **True Positive (TP):** Asli Selamat, ditebak Selamat = [Isi jumlah orang]
3. **False Positive (FP - Error Tipe I):** Asli Meninggal, tapi ditebak Selamat = [Isi jumlah orang]
4. **False Negative (FN - Error Tipe II):** Asli Selamat, tapi ditebak Meninggal = [Isi jumlah orang]

**B. Analisis Skenario Nyata (Wajib Diisi Secara Kritis):**

**Pertanyaan 1 (Skenario Titanic):** Bayangkan Anda adalah Komandan Tim SAR. Anda menggunakan AI ini untuk mencari korban setelah kapal tenggelam. Berdasarkan angka **False Positive (FP)** Anda, ada berapa orang yang aslinya tenggelam/meninggal, tetapi layar komputer Anda mengatakan *"Orang ini Selamat"*. Apa bahaya operasional dari kesalahan *False Positive* ini bagi tim SAR Anda?

> **Jawaban Kritis 1:** (Tulis analisis Anda di sini)

**Pertanyaan 2 (Skenario Medis - Kanker Payudara):**
Bandingkan dengan materi di kelas (Kanker Payudara: 0=Ganas, 1=Jinak). Dalam kasus medis, jika AI melakukan kesalahan **False Positive** (Asli Ganas, ditebak Jinak), pasien yang sakit parah akan disuruh pulang. Namun jika AI melakukan **False Negative** (Asli Jinak, ditebak Ganas), pasien sehat akan panik dan menjalani kemoterapi yang tidak perlu.
Menurut Anda, sebagai desainer sistem AI Rumah Sakit, kesalahan mana yang **lebih fatal** dan tidak boleh terjadi? Mengapa metrik "Accuracy" saja bisa menipu dan membahayakan nyawa pasien?

> **Jawaban Kritis 2:** (Tulis analisis Anda di sini)

---

## 4. Dokumentasi Eksperimen

Lampirkan *screenshot* dari *dashboard* W&B Anda yang menampilkan *bar chart* atau *line plot* dari metrik klasifikasi yang Anda kerjakan.

> **[Tempel Screenshot W&B Anda di Sini]**

---

## 5. Kesimpulan

Berdasarkan metrik dan matriks yang Anda analisis, apakah model Regresi Logistik dasar ini sudah cukup layak (*reliable*) untuk digunakan dalam sistem keselamatan nyata? Fitur tambahan apa yang mungkin bisa Anda buat (seperti *FamilySize* di Minggu 2) untuk menaikkan akurasi model ini?

> **Jawaban:** (Tulis kesimpulan Anda di sini)

---

### Instruksi Pengumpulan:

1. Isi template ini dengan pemikiran kritis Anda, jangan hanya mengandalkan teori teks.
2. Simpan sebagai **PDF** atau **Markdown** (`.md`).
3. Unggah ke *fork* repositori Anda di folder `assignments/week-4/NIM_NAMA/` beserta file *Notebook* `.ipynb` Anda.
4. Lakukan *Pull Request* ke repositori dosen.

---
