# Minggu 1: Cloud-Native Setup & Hello ML 🚀

## Tujuan Pembelajaran
1. Memahami ekosistem Cloud-Native ML (Colab, GitHub, W&B).
2. Memahami perbedaan AI vs ML vs Deep Learning secara konseptual.
3. Berhasil menjalankan "Magic Demo" pertama di cloud.

## 1. Mengapa Cloud-Native?
Di industri global, kita tidak lagi mengandalkan kekuatan laptop lokal. 
- **Scalability:** Kita bisa menyewa GPU/TPU di cloud saat butuh.
- **Reproducibility:** Kode yang jalan di Colab saya, pasti jalan di Colab Anda.
- **Collaboration:** Integrasi Git memungkinkan tim bekerja di satu codebase.

## 2. ML Lifecycle (Gambaran Besar)
1. **Data Collection:** Mencari bahan baku.
2. **EDA:** Memahami karakteristik data.
3. **Preprocessing:** Membersihkan data.
4. **Modeling:** Melatih otak buatan.
5. **Evaluation:** Menguji kecerdasan model.
6. **Deployment:** Mengirim model ke dunia nyata.

## 3. Tooling Setup
Mahasiswa wajib memiliki akun:
- **GitHub:** Untuk version control.
- **Weights & Biases (W&B):** Untuk memantau performa model secara real-time.
- **Hugging Face:** Untuk mengakses model AI tercanggih di dunia.

## Fokus Pekan Ini:
Sesuai dengan Roadmap 2026, fokus kita adalah memastikan infrastruktur pengembangan sudah siap.

1. **Cloud Setup:** Mengintegrasikan Google Colab, GitHub, dan Weights & Biases (W&B).
2. **Library Essentials:** Mengenal Scikit-learn untuk ML klasik dan Transformers untuk Modern AI.
3. **Dataset:** Menggunakan Scikit-learn Toy Datasets (Iris).

## Materi Praktikum
- [01_Hello_ML.ipynb](./01_Hello_ML.ipynb): Implementasi pertama ML dengan tracking experiment di W&B.

## Dokumentasi Pendukung
- [W&B Quickstart Guide](https://docs.wandb.ai/quickstart)
- [Scikit-learn Datasets Docs](https://scikit-learn.org/stable/datasets/toy_dataset.html)

## 📝 Tugas Minggu 1
1. **Setup Akun:** Pastikan Anda sudah mendaftar GitHub, W&B, dan Hugging Face.
2. **Clone & Run:** Buka file `01_Hello_ML.ipynb` di Colab Anda.
3. **Modifikasi:** Pada "Magic Demo 2", ganti kalimatnya dengan kalimat Bahasa Indonesia lain (misal: "Macet di Jakarta membuat saya pusing").
4. **Screenshot:** Ambil screenshot dashboard **Weights & Biases** Anda yang menunjukkan grafik akurasi dari latihan tadi.
5. **Submit:** Masukkan screenshot tersebut ke dalam folder `assignments/minggu-1/` di repositori GitHub pribadi Anda (fork dari repo ini).
