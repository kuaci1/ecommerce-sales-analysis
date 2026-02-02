# 🛒 E-Commerce Sales Analysis & Business Insights

## 📌 Gambaran Proyek
Proyek ini bertujuan untuk menganalisis dataset transaksi ritel online multinasional (UK-based) untuk periode satu tahun. Fokus utama analisis adalah mengidentifikasi **pola penjualan musiman**, **produk berkinerja tinggi**, dan **potensi pasar internasional** untuk memberikan rekomendasi strategis bagi manajemen.

Dataset mencakup transaksi dari 01/12/2010 hingga 09/12/2011 untuk pengecer online non-toko yang terdaftar di Inggris.

## 🎯 Tujuan Bisnis
1.  **Analisis Performa:** Memantau pertumbuhan pendapatan bulanan dan tren transaksi.
2.  **Produk Unggulan:** Mengidentifikasi produk "Hero" (Volume tinggi) vs "Cash Cow" (Revenue tinggi).
3.  **Ekspansi Pasar:** Menemukan negara dengan basis pelanggan terkuat di luar Inggris.
4.  **Optimasi Stok:** Memberikan rekomendasi waktu *restock* berdasarkan tren musiman.

## 🛠️ Tech Stack
* **Python:** Bahasa pemrograman utama.
* **Pandas:** Pembersihan dan manipulasi data.
* **Matplotlib & Seaborn:** Visualisasi data statis.
* **NumPy:** Operasi numerik.

## 🧹 Data Cleaning & Preprocessing
Data mentah mengandung banyak *noise*. Langkah pembersihan yang dilakukan meliputi:
* **Menghapus Transaksi Tanpa ID Pelanggan:** Menghapus baris dengan `CustomerID` kosong untuk memastikan analisis perilaku pelanggan yang akurat.
* **Handling Retur:** Menghapus transaksi pembatalan (Invoice diawali huruf 'C') dan Quantity negatif.
* **Pembersihan Anomali:** Menghapus harga unit bernilai 0 atau negatif.
* **Feature Engineering:** Membuat kolom baru `TotalRevenue` (`Quantity` * `UnitPrice`) dan ekstraksi periode bulan.

## 📊 Insight Utama (Key Findings)

### 1. Tren Musiman (Seasonality)
> **Insight:** Penjualan stabil di Q1-Q3, namun mengalami lonjakan ekstrem mulai bulan **September** dan memuncak di **November** (Persiapan Natal/Tahun Baru).
>
> **Rekomendasi:** Inventaris gudang harus ditingkatkan minimal 30-40% pada bulan Agustus untuk mencegah *stockout* di Q4.

### 2. Produk Terlaris
> **Insight:** Produk *"White Hanging Heart T-Light Holder"* adalah item dengan frekuensi transaksi tertinggi (>2000 transaksi). Ini adalah "Traffic Generator".
>
> **Rekomendasi:** Gunakan produk ini sebagai *Loss Leader* dalam kampanye iklan untuk menarik pelanggan baru.

### 3. Pasar Internasional
> **Insight:** Di luar Inggris (UK), pasar terbesar adalah **Belanda (Netherlands)** dan **Eire (Irlandia)**, diikuti oleh Jerman dan Prancis.
>
> **Rekomendasi:** Pertimbangkan untuk membangun gudang distribusi mini atau kerjasama logistik khusus di Belanda untuk menekan biaya pengiriman internasional.

## 📈 Visualisasi

*(Anda bisa memasukkan screenshot grafik yang tadi kita buat di sini)*

| Tren Bulanan | Top Produk |
| :---: | :---: |
| ![Monthly Trend](path/to/your/trend_image.png) | ![Top Products](path/to/your/product_image.png) |

## 🚀 Cara Menjalankan Project
1. Clone repositori ini:
   ```bash
   git clone [https://github.com/username-anda/ecommerce-sales-analysis.git](https://github.com/username-anda/ecommerce-sales-analysis.git)
