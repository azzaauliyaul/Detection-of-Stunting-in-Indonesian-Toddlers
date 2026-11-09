## LAMPIRAN B. FORMULIR PENGAJUAN IDE (DIKUMPULKAN PADA CHECKPOINT 1)

| Komponen | Isian Mahasiswa |
|----------|-----------------|
| Nama / NIM | Azza Auliyaul Fitri / 244311006 <br/> Edwin Nur Cahyo / 244311012|
| Judul ide | Klasifikasi Status Gizi dan Deteksi Dini Stunting pada Balita di Indonesia |
| SDG & target yang dipilih | Proyek ini berfokus pada SDG 3 (Kehidupan Sehat dan Sejahtera) dengan target mengakhiri kematian bayi dan balita yang dapat dicegah, serta mengeliminasi segala bentuk malnutrisi pada balita pada tahun 2030. |
| Masalah nyata yang diangkat | permasalahan klasifikasi gizi balita di posyandu yang masih sering dilakukan secara manual menggunakan tabel kurva standar pertumbuhan fisik yang rentan kesalahan pencatatan dan menyebabkan keterlambatan intervensi gizi pada balita yang seharusnya dikategorikan stunting. |
| Tugas ML (Target & jenis tugas) | - Tugas ML: Tabular Multi-class Classification. <br/> - klasifikasikan status gizi balita <br/> - informasi pendukung bagi kader kesehatan dalam mitgasi dini serta penentuan prioritas intervensi gizi anak. |
| Objective & metrik utama | Optimasi model dilakukan dengan meminimalkan fungsi kerugian Categorical Cross-Entropy Loss yang diintegrasikan dengan pembobotan kelas (class weights), sedangkan performa akhir dievaluasi menggunakan metrik utama Macro F1-Score untuk mengukur keseimbangan prediksi antar-kelas secara adil serta Recall pada kategori rentan (Stunted dan Severely Stunted) guna meminimalkan risiko kesalahan deteksi balita stunting sebagai normal (false negative). |
| Dataset (sumber, URL, ukuran, jenis data) | - [Stunting Toddler (Balita) Detection (121K rows)](https://www.kaggle.com/datasets/rendiputra/stunting-balita-detection-121k-rows) |
| Rencana tiga model (baseline / advanced / deep learning) | - Baseline Model: Multinomial Logistic Regression <br/> - Advanced Model: LightGBM Classifier <br/> - Deep Learning Model: Multilayer Perceptron (MLP)|
| Risiko & pertimbangan etika (bias, privasi) | Kesalahan prediksi, khususnya false negative (balita stunting terprediksi normal), dapat menyebabkan keterlambatan penanganan medis yang berdampak pada tumbuh kembang anak |
| Referensi awal (minimal 2) | [COMPARISON OF RANDOM FOREST, K-NEAREST NEIGHBOR, DECISION TREE, AND XGBOOST ALGORITHMS FOR DETECTING STUNTING IN TODDLERS](https://doi.org/10.52436/1.jutif.2024.5.6.2629) <br/><br/>[Analisis Perbandingan Algoritma SVM, Random Forest dan Logistic Regression untuk Prediksi Stunting Balita](https://doi.org/10.29408/edumatic.v9i1.29407) |

**Kriteria persetujuan dosen:**
- [ ] Ide berasal dari mahasiswa dan tidak duplikat
- [ ] Selaras jelas dengan satu SDG dan targetnya
- [ ] Dapat dirumuskan sebagai masalah ML dengan target yang jelas
- [ ] Dataset tersedia, legal/etis digunakan, dan cukup besar
- [ ] Layak untuk tiga model termasuk deep learning dalam 6 minggu
