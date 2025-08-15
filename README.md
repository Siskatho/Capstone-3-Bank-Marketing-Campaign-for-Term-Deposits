# Capstone-3-Bank-Marketing-Campaign-for-Term-Deposits
Bank Marketing Analytics: Bank Marketing Campaign for Term Deposits

Background
Proyek ini menerapkan Machine Learning untuk memprediksi apakah seorang nasabah bank akan berlangganan produk deposito berjangka.
Dengan memprediksi minat nasabah, bank dapat mengoptimalkan biaya kampanye dan mengurangi peluang yang hilang.

---

Business Problem
Bank menghadapi dua strategi pemasaran yang kurang efisien:
Target All – Biaya kampanye tinggi karena menghubungi nasabah yang tidak tertarik.
Target None – Kehilangan pendapatan besar karena tidak menghubungi nasabah yang sebenarnya tertarik.

Tujuan proyek ini adalah membangun model prediksi yang mengidentifikasi nasabah dengan kemungkinan tinggi untuk membuka deposito berjangka, sehingga meningkatkan efisiensi penargetan.

---

Tujuan
Meningkatkan efisiensi pemasaran.
Mengurangi biaya Campaign yang tidak perlu.
Meminimalkan peluang yang hilang dengan mengidentifikasi nasabah berpotensi tinggi.

---

Dataset
Sumber: Bank-Marketing-Campaign-for-Term-Deposits
Google Drive
Fitur Utama
| Fitur | Deskripsi |
|-------|-----------|
| age | Usia nasabah |
| job | Jenis pekerjaan |
| balance | Saldo rekening |
| housing | Status pinjaman rumah |
| loan | Status pinjaman pribadi |
| contact | Jenis komunikasi |
| month | Bulan kontak terakhir |
| campaign | Jumlah kontak selama kampanye |
| pdays | Hari sejak kontak terakhir pada kampanye sebelumnya |
| poutcome | Hasil kampanye sebelumnya |
| deposit | Variabel target (yes/no) |

---

Metodologi
Pembersihan & Pra-pemrosesan Data
Menangani nilai yang hilang/tidak diketahui.
Melakukan encoding variabel kategorikal.
Melakukan scaling pada fitur numerik.

Pemodelan
Mencoba beberapa algoritma klasifikasi: Logistic Regression, Decision Tree, KNN, Random Forest, Gradient Boosting, AdaBoost.
Metrik evaluasi: F-β score (β=3) untuk memprioritaskan recall.

Evaluasi Model
Membandingkan performa model dengan strategi dasar.
Memilih model dengan recall tertinggi sambil menjaga biaya tetap efisien.

---

Hasil
Model ML mengungguli strategi dasar dalam hal efisiensi biaya.
Mengurangi pemborosan biaya kampanye dan meminimalkan peluang yang hilang.
Memiliki nilai recall tinggi, memastikan sebagian besar calon nasabah potensial dapat ditargetkan.

---

Rekomendasi
Mengumpulkan data yang lebih beragam dan terkini.
Mengeksplorasi metode ensemble lanjutan (XGBoost, LightGBM).
Menangani ketidakseimbangan kelas melalui oversampling atau fungsi loss berbobot.
Menerapkan model ke produksi untuk prediksi real-time.

---

Kesimpulan
Model ini memberikan strategi penargetan berbasis data untuk kampanye pemasaran bank.
Model ini menunjukkan potensi yang jelas untuk penghematan biaya dan peningkatan ROI kampanye, dibandingkan dengan pendekatan penargetan massal tradisional.

---

Persyaratan
Python 3.9+
pandas, numpy, matplotlib, seaborn
scikit-learn
category_encoders
