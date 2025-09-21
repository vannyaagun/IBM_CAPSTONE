# 🌍 Capstone Project: Analisis & Prediksi Bencana Alam di Indonesia

## 📌 Project Overview
Indonesia merupakan negara rawan bencana karena faktor geografis dan iklim tropisnya.  
Proyek ini bertujuan untuk:
- Menganalisis pola historis bencana di Indonesia.
- Mengidentifikasi faktor risiko utama.
- Membuat prediksi tren bencana di masa depan.
- Melakukan **clustering** berdasarkan *severity* dan *lokasi*.
- Menghasilkan **summarization otomatis** berisi pola historis, hasil clustering, prediksi, dan rekomendasi mitigasi.

---

## 📊 Raw Dataset
Dataset berasal dari BNPB (via Kaggle):

🔗 [Indonesia Natural Disaster Dataset (BNPB Records)](https://www.kaggle.com/datasets/maudiana/indonesia-natural-disaster-dataset-bnpb-records)

Dataset ini berisi informasi:
- **Tanggal/Waktu kejadian**  
- **Jenis bencana** (banjir, gempa bumi, longsor, dll.)  
- **Lokasi kejadian** (provinsi & kota)  
- **Dampak bencana** (jumlah korban, rumah rusak, fasilitas terdampak)  

---

## 📈 Insight & Findings
Beberapa insight utama dari hasil analisis:

### 🔹 Distribusi Temporal
- Jumlah bencana meningkat pada **musim hujan (Januari–Maret)**.
- Tren musiman terlihat konsisten tiap tahun.

### 🔹 Jenis Bencana Paling Umum
- **Banjir** → paling sering terjadi.  
- **Tanah Longsor, Cuaca Ekstrem, Kebakaran Hutan** → juga cukup dominan.  

### 🔹 Lokasi Rawan
- **Jawa Tengah, Kalimantan Selatan, NTT, Bali** adalah wilayah dengan frekuensi tinggi.  

### 🔹 Penyebab
- Faktor alam: **curah hujan tinggi, erosi tanah, gempa**.  
- Faktor manusia: **pembakaran lahan, kelalaian industri**.  

### 🔹 Dampak
- **Bencana frekuensi tinggi** (banjir, longsor) → merusak infrastruktur.  
- **Bencana frekuensi rendah** (tsunami, erupsi) → korban jiwa lebih besar.  

### 🔹 Clustering
- **Cluster ringan** → korban & kerusakan minim.  
- **Cluster sedang** → dampak menengah.  
- **Cluster berat** → korban jiwa tinggi, infrastruktur rusak parah.  

---

## 🤖 AI Support Explanation
Proyek ini menggunakan kombinasi **LangChain + LLM** dan metode AI lain untuk mempercepat analisis:

- **LangChain + LLM (Granite 3.3-8B)**  
  - Query dataframe otomatis dengan bahasa natural.  
  - Membersihkan data (missing values, normalisasi nama provinsi/kota).  

- **Exploratory Data Analysis (EDA)**  
  - Visualisasi tren bulanan (line chart).  
  - Jenis bencana (pie chart).  
  - Lokasi & penyebab (bar chart, heatmap).  

- **Clustering (K-Means / DBSCAN)**  
  - Mengelompokkan bencana berdasarkan severity & lokasi.  

- **Time Series Forecasting (ARIMA / Prophet)**  
  - Memprediksi jumlah bencana bulanan ke depan dengan pola musiman.  

- **Summarization (LLM)**  
  - Menghasilkan ringkasan historis, clustering, prediksi, dan rekomendasi mitigasi.  

✅ **Manfaat AI:** mempercepat analisis big data, mengekstrak pola musiman, dan menghasilkan insight yang actionable.  

---

## 📌 Conclusion & Recommendations
- **Kesimpulan:**  
  Bencana di Indonesia memiliki pola musiman, dengan puncak pada awal tahun.  
  Banjir, longsor, dan kebakaran hutan adalah jenis bencana dominan.  
  Clustering mengungkap wilayah rawan dan tingkat keparahan bencana.  

- **Rekomendasi:**  
  - Fokus mitigasi di bulan rawan (Januari–Maret).  
  - Perkuat infrastruktur di wilayah cluster "berat".  
  - Edukasi & early warning di cluster "ringan".  
  - Perbaiki drainase (banjir), lakukan reboisasi (longsor), dan pengendalian lahan (kebakaran).  

---

## 👨‍💻 Author
Vannya Ade Gunawan  
21-09-2025  
