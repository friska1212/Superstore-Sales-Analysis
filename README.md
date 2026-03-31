# 📊 Superstore Sales Analysis

**Minggu 6 — Reporting & Data Storytelling**
Laporan Analisis Bisnis menggunakan Dataset Superstore Retail Amerika Serikat

---

## 📌 Project Overview

Proyek ini bertujuan untuk menganalisis performa penjualan dan profit pada bisnis retail menggunakan Dataset Superstore. Analisis dilakukan untuk menemukan insight bisnis yang dapat membantu pengambilan keputusan strategis, mencakup analisis berdasarkan region, kategori produk, dan dampak diskon terhadap profitabilitas.

---

## 📊 Data Understanding

Dataset yang digunakan merupakan data transaksi penjualan retail Amerika Serikat dengan detail sebagai berikut:

| Metrik | Nilai |
|--------|-------|
| Total Baris Data | 9.994 transaksi |
| Total Kolom | 21 kolom |
| Total Sales | $2.297.200 |
| Total Profit | $286.397 |
| Wilayah | 4 Region (East, West, Central, South) |
| Kategori Produk | 3 Kategori, 17 Sub-Kategori |

### Kolom Utama yang Digunakan:

| Kolom | Deskripsi |
|-------|-----------|
| Region | Wilayah penjualan (East, West, Central, South) |
| Category | Kategori produk (Furniture, Technology, Office Supplies) |
| Sub-Category | Sub-kategori produk (17 sub-kategori) |
| Sales | Total nilai penjualan per transaksi |
| Profit | Keuntungan per transaksi (bisa negatif) |
| Discount | Besaran diskon yang diberikan (0–80%) |

---

## 🧹 Data Cleaning

Proses data cleaning dilakukan langsung pada file kerja dengan langkah-langkah berikut:

- Penyesuaian nama dan format kolom
- Pengecekan missing value
- Pengecekan data duplikat
- Validasi tipe data pada kolom numerik (Sales, Profit, Discount)

---

## 📈 Exploratory Data Analysis

### 1. Sales Analysis — by Region

Analisis distribusi penjualan di setiap wilayah (region) untuk memahami kontribusi tiap region terhadap total penjualan.

| Region | Total Sales | Share |
|--------|-------------|-------|
| West | $725.458 | 30,6% |
| East | $678.781 | 28,6% |
| Central | $501.240 | 21,1% |
| South | $391.722 | 16,5% |

West & East menyumbang 59,2% dari total penjualan.

---

### 2. Profit Analysis — by Category

Analisis profit berdasarkan kategori produk untuk mengidentifikasi kategori mana yang paling menguntungkan.

| Kategori | Total Profit | Margin |
|----------|-------------|--------|
| Technology | $145.455 | 17,4% |
| Office Supplies | $122.491 | 17,4% |
| Furniture | $18.451 | 2,5% |

Furniture perlu evaluasi — sales tinggi namun margin profit sangat rendah (2,5%).

---

### 3. Discount Analysis — Dampak Diskon terhadap Profit

Analisis hubungan antara tingkat diskon yang diberikan dengan rata-rata profit per transaksi.

| Range Diskon | Avg Profit |
|-------------|-----------|
| 0% | +$168,83 |
| 1–10% | +$55,31 |
| 11–20% | +$26,42 |
| 21–30% | -$13,56 |
| 31–40% | -$89,23 |
| 41–50% | -$142,67 |
| 51%+ | -$198,45 |

Temuan Kunci:
- Tanpa diskon (0%) = profit rata-rata tertinggi ($168)
- Diskon 21–30% mulai menghasilkan profit negatif
- Diskon 31%+ selalu menghasilkan kerugian
- 1.871 transaksi mengalami profit negatif

Batas aman diskon adalah maksimal 20% untuk tetap menjaga profit positif.

---

## 💡 Key Insights

1. West & East mendominasi — dua region ini menyumbang 59% dari total sales, sementara South hanya berkontribusi 16,5%
2. Technology paling profitable — margin 17,4%, menjadikannya kategori terbaik untuk difokuskan
3. Furniture butuh perhatian — walaupun punya banyak transaksi, margin profitnya hanya 2,5%
4. Diskon merugikan bisnis — diskon di atas 20% terbukti menghasilkan profit negatif
5. Phones & Chairs = sub-kategori terlaris — perlu strategi khusus untuk memaksimalkan potensinya

---

## 🎯 Business Recommendation

| # | Rekomendasi |
|---|------------|
| Rec #1 | Batasi diskon maksimal 20% untuk menjaga profitabilitas |
| Rec #2 | Fokus tingkatkan penjualan Technology di semua region |
| Rec #3 | Evaluasi strategi pricing Furniture — margin terlalu tipis |
| Rec #4 | Investasikan lebih banyak di region South yang masih potensial |

---

