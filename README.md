# 📦 Amazon Sales Analytics Dashboard 2022

Analisis terhadap **128.000+ transaksi penjualan Amazon India** periode April–Juni 2022 untuk menjawab pertanyaan bisnis seputar performa revenue, kategori produk, dan efisiensi pengiriman.

> **Tools:** Python (Pandas) · MySQL · Power BI

---

## ❓ Pertanyaan Bisnis

1. Kategori produk mana yang menghasilkan revenue terbesar?
2. Bagaimana tren revenue harian selama April–Juni 2022?
3. Seberapa efisien proses fulfillment order?
4. Berapa total Gross Merchandise Value (GMV) keseluruhan?

---

## 📊 Ringkasan Metrik

| Metrik | Nilai |
|--------|-------|
| Gross Merchandise Value (GMV) | ₹78.59M (INR) |
| Total Order | 128.975 transaksi |
| Kategori Terlaris | Set — ₹39M (~50% GMV) |
| Order Terkirim | 60.32% |
| Cancellation Rate | 14.21% |

---

## 💡 Key Findings & Insight

### 1. Kategori Set Mendominasi Pasar
Kategori **Set** menyumbang hampir **50% dari total GMV** (₹39M dari ₹78.59M), jauh melampaui Kurta di posisi kedua (₹21M). Ini mengindikasikan bahwa pakaian set/koordinat adalah produk andalan yang perlu dijaga stok dan promosinya secara konsisten.

### 2. Revenue Menurun Signifikan April → Juni
Tren harian menunjukkan **puncak revenue di pertengahan April 2022**, kemudian turun secara konsisten hingga akhir Juni. Penurunan ini kemungkinan disebabkan oleh berakhirnya periode promosi atau campaign musiman. Perlu investigasi lebih lanjut apakah ada event/diskon besar di April yang mendorong lonjakan tersebut.

### 3. Cancellation Rate 14.21% — Area yang Perlu Diperhatikan
Lebih dari **1 dari 7 order dibatalkan**. Angka ini cukup signifikan dan berpotensi menjadi kebocoran revenue. Penyebab umum biasanya: stok habis setelah order masuk, keterlambatan konfirmasi, atau masalah harga. Investigasi lebih dalam per kategori bisa membantu menemukan akar masalahnya.

### 4. 60.32% Order Masih Berstatus "Shipped"
Mayoritas order tercatat sebagai **Shipped tanpa konfirmasi Delivered**. Ini bisa mengindikasikan gap dalam sistem tracking pengiriman — data status pengiriman tidak terupdate secara real-time. Hanya **22.31% yang terkonfirmasi sampai ke pembeli**.

---

## 📸 Dashboard

![Dashboard Preview](dashboard_preview.png)

---

## 🔧 Teknis Singkat

Data diproses melalui pipeline **ETL** (Extract → Transform → Load):
- **Extract** — Dataset CSV dari Kaggle (128K baris)
- **Transform** — Pembersihan data dengan Python & Pandas (handling missing values, format tanggal, rename kolom)
- **Load** — Disimpan ke database MySQL
- **Visualize** — Dashboard interaktif di Power BI

---

<div align="center">

**Dea Alensa** · [github.com/deaalensa](https://github.com/deaalensa) · 2026

</div>
