# UTS Machine Learning — Jalur A (Klasifikasi)

## Identitas Mahasiswa
- **Nama:** I Gede Diky Saputra
- **NIM:** 2301010515
- **Kelas / Semester:** Ganjil / XX 
- **Program Studi:** Informatika — Institut Bisnis dan Teknologi Indonesia (INSTIKI)
- **Variabel `SEED`:** `515` 

## Ringkasan Proyek
Proyek ini menerapkan alur **CRISP-DM** pada **Jalur A (Klasifikasi)** menggunakan dataset `dataset1.csv` (880 baris, 12 fitur numerik parameter kimia/kesuburan tanah, dan 1 target kategori `Output` dengan kelas `0`, `1`, dan `2`). Model utama dibangun menggunakan `Pipeline` dan `ColumnTransformer` bebas kebocoran data dengan pembagian data terstratifikasi (`stratify=y`) serta validasi silang *5-fold StratifiedKFold*, membandingkan `DummyClassifier` (*baseline*), `KNeighborsClassifier` (KNN), `SVC` (SVM RBF), dan `GaussianNB`.

## Sumber, Lisensi, dan Privasi Data
- **Nama / File Dataset:** `dataset1.csv`
- **Link Sumber:** *[Isi link sumber dataset resmi tempat file diunduh/didaftarkan di ELSA]*
- **Tanggal Akses:** *[Isi tanggal akses saat mengunduh dataset]*
- **Lisensi:** *[Cantumkan lisensi dataset sesuai halaman sumbernya]*
- **Kepatuhan Privasi:** Dataset berisi parameter kimia dan kesuburan tanah (`N`, `P`, `K`, `pH`, `EC`, `OC`, `S`, `Zn`, `Fe`, `Cu`, `Mn`, `B`, `Output`) dan tidak memuat data identitas pribadi.

## Pernyataan Penggunaan AI
- **Alat yang dipakai:** Gemini
- **Bagian yang dibantu:** Penyusunan alur tahapan 1–6 Jalur A, kode eksplorasi data, pra-pemrosesan (`Pipeline` & `ColumnTransformer`), pemodelan dan evaluasi metrik, perhitungan manual metrik dari *confusion matrix*, serta draf dokumentasi `README.md`.
- **Cara memeriksa hasil:** Seluruh sel notebook dijalankan secara berurutan (`Runtime -> Run all`), hasil metrik dan *confusion matrix* diverifikasi langsung dari output eksekusi kode, serta setiap bagian kode dipahami dan disesuaikan agar dapat dijelaskan maupun diubah saat sesi presentasi/tanya jawab.

## Struktur Repositori
```text
UTS-ML-2301010515-I-Gede-Diky-Saputra/
├── README.md
├── notebook/
│   └── UTS_ML_2301010515_IGedeDikySaputra.ipynb
├── data/
│   └── dataset1.csv
└── reports/
    ├── 01_distribusi_target_fitur.png
    ├── 02_korelasi_dan_boxplot.png
    └── 03_cv_dan_confusion_matrix.png
```

## Cara Menjalankan Notebook
1. Buka `notebook/UTS_ML_2301010515_IGedeDikySaputra.ipynb` di Google Colab atau Jupyter Notebook.
2. Pastikan file `dataset1.csv` tersedia pada path yang sesuai (`../data/dataset1.csv` jika menggunakan struktur folder di atas).
3. Jalankan seluruh sel secara berurutan melalui **Runtime -> Run all** dan pastikan seluruh output serta grafik tersimpan dengan baik sebelum melakukan *commit* terakhir ke GitHub.