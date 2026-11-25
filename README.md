# UTS Machine Learning — Jalur A (Klasifikasi)

## Identitas Mahasiswa

- **Nama:** I Gede Diky Saputra
- **NIM:** 2301010515
- **Kelas / Semester:** Ganjil / XX
- **Program Studi:** Informatika — Institut Bisnis dan Teknologi Indonesia (INSTIKI)
- **Variabel `SEED`:** `515`

## Ringkasan Proyek

Proyek ini menerapkan alur **CRISP-DM** pada **Jalur A (Klasifikasi)** menggunakan dataset `dataset1.csv` (880 baris, 12 fitur numerik parameter kimia/kesuburan tanah, dan 1 target kategori `Output` dengan kelas `0`, `1`, dan `2`). Model utama dibangun menggunakan `Pipeline` dan `ColumnTransformer` bebas kebocoran data dengan pembagian data terstratifikasi (`stratify=y`) serta validasi silang _5-fold StratifiedKFold_, membandingkan `DummyClassifier` (_baseline_), `KNeighborsClassifier` (KNN), `SVC` (SVM RBF), dan `GaussianNB`.

## Sumber, Lisensi, dan Privasi Data

- **Nama / File Dataset:** `dataset1.csv`
- **Link Sumber:** _[Isi link sumber dataset resmi tempat file diunduh/didaftarkan di ELSA]_
- **Tanggal Akses:** _[Isi tanggal akses saat mengunduh dataset]_
- **Lisensi:** _[Cantumkan lisensi dataset sesuai halaman sumbernya]_
- **Kepatuhan Privasi:** Dataset berisi parameter kimia dan kesuburan tanah (`N`, `P`, `K`, `pH`, `EC`, `OC`, `S`, `Zn`, `Fe`, `Cu`, `Mn`, `B`, `Output`) dan tidak memuat data identitas pribadi.

## Pernyataan Penggunaan AI

- **Alat yang dipakai:** Gemini
- **Bagian yang dibantu:** Penyusunan alur tahapan 1–6 Jalur A, kode eksplorasi data, pra-pemrosesan (`Pipeline` & `ColumnTransformer`), pemodelan dan evaluasi metrik, perhitungan manual metrik dari _confusion matrix_, serta draf dokumentasi `README.md`.
- **Cara memeriksa hasil:** Seluruh sel notebook dijalankan secara berurutan (`Runtime -> Run all`), hasil metrik dan _confusion matrix_ diverifikasi langsung dari output eksekusi kode, serta setiap bagian kode dipahami dan disesuaikan agar dapat dijelaskan maupun diubah saat sesi presentasi/tanya jawab.
