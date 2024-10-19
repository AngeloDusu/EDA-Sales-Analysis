# E-Commerce Sales Analysis

## Project Overview / Ringkasan Proyek
This project involves analyzing an E-commerce Sales Dataset to understand sales trends, identify best-selling products, examine customer demographics, and assess customer retention. Through exploratory data analysis (EDA), various insights will be derived to provide business recommendations.

Proyek ini melibatkan analisis Dataset Penjualan E-commerce untuk memahami tren penjualan, mengidentifikasi produk terlaris, memeriksa demografi pelanggan, dan menilai retensi pelanggan. Melalui analisis data eksploratif (EDA), berbagai wawasan akan dihasilkan untuk memberikan rekomendasi bisnis.

## Objectives / Tujuan
- Analyze sales trends over time.
- Identify top-selling products and categories.
- Analyze customer demographics and behavior.
- Evaluate customer retention and churn.
- Make business recommendations based on data insights.

- Menganalisis tren penjualan dari waktu ke waktu.
- Mengidentifikasi produk dan kategori terlaris.
- Menganalisis demografi dan perilaku pelanggan.
- Mengevaluasi retensi dan churn pelanggan.
- Memberikan rekomendasi bisnis berdasarkan wawasan data.

## Tools Used / Alat yang Digunakan
- **Python**: Pandas, Matplotlib, Seaborn
- **Jupyter Notebook**: For writing code and visualizing results
- **Git**: Version control and project collaboration
- **GitHub**: Hosting project repository

- **Python**: Pandas, Matplotlib, Seaborn
- **Jupyter Notebook**: Untuk menulis kode dan memvisualisasikan hasil
- **Git**: Kontrol versi dan kolaborasi proyek
- **GitHub**: Menampung repositori proyek

## Folder Structure / Struktur Folder
```bash
|-- EDA-Sales-Analysis/
    |-- data/                # Dataset folder / Folder dataset
    |-- notebooks/           # Jupyter notebooks for EDA and analysis / Jupyter notebook untuk EDA dan analisis
    |-- src/                 # Python scripts (if necessary) / Skrip Python (jika perlu)
    |-- output/              # Visualizations and reports / Visualisasi dan laporan
    |-- README.md            # Project overview and details / Ringkasan dan detail proyek
    |-- requirements.txt     # List of dependencies (if necessary) / Daftar ketergantungan (jika perlu)
```

## Steps of Exploratory Data Analysis (EDA) / Langkah-langkah Analisis Data Eksploratif (EDA)

### Data Cleaning / Pembersihan Data
- Remove or handle missing data.
- Convert data types (e.g., date formatting).
- Handle outliers and incorrect values.

- Menghapus atau menangani data yang hilang.
- Mengonversi tipe data (misalnya, format tanggal).
- Menangani outlier dan nilai yang salah.

### Understanding the Data / Memahami Data
- Get an overview of the dataset (e.g., data types, number of rows, columns).
- Use `df.describe()` and `df.info()` to summarize the dataset.

- Mendapatkan gambaran umum dataset (misalnya, tipe data, jumlah baris, kolom).
- Menggunakan `df.describe()` dan `df.info()` untuk merangkum dataset.

### Univariate Analysis / Analisis Univariate
- Analyze individual columns/features.
- Example: Distribution of sales in different product categories.

- Menganalisis kolom/fitur individu.
- Contoh: Distribusi penjualan dalam berbagai kategori produk.

### Multivariate Analysis / Analisis Multivariate
- Analyze relationships between two or more variables.
- Example: Sales amount vs. customer age.

- Menganalisis hubungan antara dua atau lebih variabel.
- Contoh: Jumlah penjualan vs. umur pelanggan.

### Sales Trend Over Time / Tren Penjualan Seiring Waktu
- Plot sales trends over weeks, months, and years.
- Visualize sales by day or month using line plots.

- Memplot tren penjualan selama minggu, bulan, dan tahun.
- Memvisualisasikan penjualan per hari atau bulan menggunakan grafik garis.

### Top-Selling Products / Produk Terlaris
- Identify top-selling products by total revenue and units sold.
- Create bar charts to visualize top categories and products.

- Mengidentifikasi produk terlaris berdasarkan total pendapatan dan unit yang terjual.
- Membuat grafik batang untuk memvisualisasikan kategori dan produk teratas.

### Customer Segmentation / Segmentasi Pelanggan
- Segment customers based on demographics such as age, location, or gender.
- Perform group-by operations to understand customer preferences.

- Mensegmentasikan pelanggan berdasarkan demografi seperti umur, lokasi, atau jenis kelamin.
- Melakukan operasi `group-by` untuk memahami preferensi pelanggan.

### Geographical Analysis / Analisis Geografis
- Analyze customer locations and sales by region.
- Visualize sales distribution across different cities or regions.

- Menganalisis lokasi pelanggan dan penjualan berdasarkan wilayah.
- Memvisualisasikan distribusi penjualan di berbagai kota atau wilayah.

### Customer Retention and Churn Analysis / Analisis Retensi dan Churn Pelanggan
- Analyze repeat customers vs. one-time customers.
- Investigate customer churn using retention rates.

- Menganalisis pelanggan yang berulang vs. pelanggan satu kali.
- Menyelidiki churn pelanggan menggunakan tingkat retensi.

### Correlation Analysis / Analisis Korelasi
- Examine relationships between numerical variables.
- Use correlation heatmaps to visualize strong and weak correlations.

- Memeriksa hubungan antara variabel numerik.
- Menggunakan heatmap korelasi untuk memvisualisasikan korelasi yang kuat dan lemah.

## Visualizations / Visualisasi

### Sales Distribution by Product Line / Distribusi Penjualan Berdasarkan Kategori Produk:
KDE plot showing sales distribution across product lines.

```python
plt.figure(figsize=(10,6))
for product in data['Product line'].unique():
    subset = data[data['Product line'] == product]
    sns.kdeplot(subset['Total'], label=product)
plt.title('Distribution of Sales by Product Line')
plt.xlabel('Total Sales')
plt.ylabel('Density')
plt.legend()
plt.show()
```

## Notes / Catatan
- **Dataset**: The dataset used for this analysis can be found in the `data/` folder.
- **Dataset**: Dataset yang digunakan untuk analisis ini dapat ditemukan di folder `data/`.

- **Further Improvements**: Future work may involve deeper analysis of customer lifetime value (CLV) and predictive modeling.
- **Perbaikan Lebih Lanjut**: Pekerjaan mendatang dapat melibatkan analisis yang lebih mendalam tentang nilai umur pelanggan (CLV) dan pemodelan prediktif.






