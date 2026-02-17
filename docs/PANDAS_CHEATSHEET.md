# 🐼 Pandas Cheat Sheet for Machine Learning

Panduan ringkas manipulasi data menggunakan library Pandas untuk kurikulum **Machine Learning 2026**.

## 1. Memuat & Inspeksi Data

Langkah pertama untuk mengenal "bahan baku" sebelum diolah.

* **Load CSV**: `df = pd.read_csv('url_atau_path')` — Membaca data dari file atau link.


* **Lihat Atas**: `df.head()` — Menampilkan 5 baris pertama data.


* **Struktur Data**: `df.info()` — Melihat tipe data dan jumlah baris/kolom.


* **Deteksi Data Kosong**: `df.isnull().sum()` — Menghitung jumlah `NaN` di setiap kolom.



---

## 2. Pembersihan Data (*Data Cleaning*)

Menangani data yang "kotor" agar model ML dapat berjalan stabil.

* **Isi Data Kosong (Imputasi)**:
* `df['kolom'].fillna(nilai, inplace=True)` — Mengisi data kosong dengan nilai tertentu.


* `df['kolom'].median()` — Mengambil nilai tengah (cocok untuk data angka yang memiliki pencilan).


* `df['kolom'].mode()[0]` — Mengambil nilai yang paling sering muncul (cocok untuk data kategori).




* **Hapus Kolom**: `df.drop(columns=['nama_kolom'], inplace=True)` — Membuang fitur yang tidak relevan atau terlalu banyak data kosong.



---

## 3. Transformasi Data (*Feature Engineering*)

Mengubah data mentah menjadi informasi yang bisa dimengerti oleh algoritma.

* **Membuat Kolom Baru**: `df['Baru'] = df['A'] + df['B']` — Operasi matematika antar kolom.


* **Mapping Kategori**: `df['Sex'].map({'male': 0, 'female': 1})` — Mengubah teks menjadi angka biner.


* **Encoding Kategori**: `df['kolom'].astype('category').cat.codes` — Mengubah banyak label kategori menjadi angka (0, 1, 2, dst).



---

## 4. Analisis & Eksplorasi

Mencari pola dan hubungan antar variabel.

* **Statistik Deskriptif**: `df.describe()` — Ringkasan cepat (mean, min, max, std).
* **Korelasi**: `df.corr(numeric_only=True)` — Melihat hubungan linier antar fitur.


* **Visualisasi Cepat**: `df['kolom'].hist()` — Melihat distribusi data secara instan.

---

### Tips untuk Mahasiswa

> "Gunakan `.copy()` saat menduplikasi DataFrame agar perubahan tidak merusak data asli, dan selalu cek `.info()` setelah melakukan `.fillna()` untuk memastikan tidak ada lagi data yang tertinggal."

---
