# KLASIFIKASI STATUS GIZI DAN DETEKSI DINI STUNTING PADA BALITA DI INDONESIA

Repositori ini memuat eksperimen model klasifikasi status gizi dan deteksi dini risiko *stunting* pada balita berbasis parameter antropometri. Seluruh pengembangan disusun mengacu pada kerangka kerja siklus hidup *Machine Learning* L-M-O-P (*Learning Problem*, *Model Design*, *Optimization*, *Predict & Evaluate*).

---

## SUMBER DATASET

Dataset yang digunakan dalam penelitian ini adalah dataset sekunder publik dari Kaggle:
- **Nama Dataset:** *Stunting Balita Detection (121k rows)*
- **Kreator:** Rendi Putra
- **Jumlah Data:** 121.000 observasi
- **Tautan Dataset:** [Kaggle - Stunting Balita Detection](https://www.kaggle.com/datasets/rendiputra/stunting-balita-detection-121k-rows)

---

## ANGGOTA TIM / KELOMPOK

**Nama Kelompok:** 9

| No. | Nama Anggota | NIM |
| :---: | :--- | :--- |
| 1. | Azza Auliyaul Fitri | 244311006 |
| 2. | Edein Nur Cahyo | 244311012 | 

---

## DAFTAR PUSTAKA DAN BERKAS DOKUMEN

Struktur direktori dokumentasi pada folder `docs/` dirinci sebagai berikut:
- [`docs/09_LAMPIRAN_B.md`](docs/09_LAMPIRAN_B.md) Formulir pengajuan ide checkpoint 1 yang memuat rumusan target klasifikasi multikelas status gizi, tautan dataset Kaggle (121k rows), rencana tiga model komparatif, analisis keterkaitan dengan SDG 3 (Target 3.2), mitigasi risiko etika (*false negative*), dan referensi ilmiah.
- [`docs/09_minggu9.md`](docs/09_minggu9.md) Panduan capaian tugas dan kriteria checkpoint tahap awal untuk perumusan masalah pembelajaran (*Learning Problem*).
- [`docs/Laporan_Proyek_ML_LMOP.md`](docs/Laporan_Proyek_ML_LMOP.md) Draf utama template laporan komprehensif dari Bab 1 hingga Bab 10 yang mencakup seluruh alur siklus hidup proyek L-M-O-P.

---

## RINGKASAN PROYEK

Proyek riset ini bertujuan menyediakan instrumen pendukung keputusan (*clinical decision support system*) bagi kader posyandu dan tenaga kesehatan untuk mengklasifikasikan status gizi balita secara cepat, objektif, dan presisi guna memitigasi risiko *stunting* sejak dini. Pendekatan komputasi membandingkan tiga tingkatan model secara bertahap:
- **Baseline Model:** *Multinomial Logistic Regression* untuk mengevaluasi korelasi linear dasar antara variabel antropometri (umur, jenis kelamin, dan tinggi badan) dengan kategori status gizi.
- **Advanced Model:** *LightGBM Classifier* berbasis *gradient boosting* untuk memetakan hubungan non-linear antarvariabel secara cepat dan efisien pada data terstruktur skala besar.
- **Deep Learning Model:** *Multilayer Perceptron* (MLP) dengan arsitektur jaringan saraf tiruan teratur menggunakan fungsi aktivasi, *Batch Normalization*, serta *Dropout* guna mereduksi risiko *overfitting* serta mempelajari representasi fitur kompleks pada data tabular.
