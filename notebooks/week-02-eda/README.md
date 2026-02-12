# Minggu 2: Data Wrangling & Interactive EDA 🚢

## Tujuan Pembelajaran
1. **Data Loading:** Membaca data langsung dari Cloud (URL GitHub).
2. **Data Cleaning:** Teknik imputasi cerdas untuk *Missing Values*.
3. **Interactive EDA:** Menggunakan **W&B Tables** untuk eksplorasi data secara visual.
4. **Feature Engineering:** Transformasi data mentah menjadi fitur siap latih.

## Konsep Utama
- **Garbage In, Garbage Out:** Kualitas model ML sangat bergantung pada kebersihan data.
- **Handling Missing Values:**
    - *Imputasi Median:* Untuk data numerik yang memiliki pencilan (outliers).
    - *Imputasi Modus:* Untuk data kategori.
- **W&B Artifacts:** Menyimpan snapshot data "bersih" agar eksperimen dapat direproduksi (reproducible).

## Dataset
Kita menggunakan **Titanic Dataset**. Data ini dipilih karena memiliki kompleksitas yang pas untuk pemula: data teks, angka, dan banyak data yang hilang.
