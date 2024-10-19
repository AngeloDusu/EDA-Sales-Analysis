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



Steps of Exploratory Data Analysis (EDA) / Langkah-langkah Analisis Data Eksploratif (EDA)
Data Cleaning

Remove or handle missing data.

Convert data types (e.g., date formatting).

Handle outliers and incorrect values.

Pembersihan Data

Menghapus atau menangani data yang hilang.

Mengonversi tipe data (misalnya, format tanggal).

Menangani outlier dan nilai yang salah.

Understanding the Data

Get an overview of the dataset (e.g., data types, number of rows, columns).

Use df.describe() and df.info() to summarize the dataset.

Memahami Data

Mendapatkan gambaran umum dataset (misalnya, tipe data, jumlah baris, kolom).

Menggunakan df.describe() dan df.info() untuk merangkum dataset.

Univariate Analysis

Analyze individual columns/features.

Example: Distribution of sales in different product categories.

Analisis Univariate

Menganalisis kolom/fitur individu.

Contoh: Distribusi penjualan dalam berbagai kategori produk.

Multivariate Analysis

Analyze relationships between two or more variables.

Example: Sales amount vs. customer age.

Analisis Multivariate

Menganalisis hubungan antara dua atau lebih variabel.

Contoh: Jumlah penjualan vs. umur pelanggan.

Sales Trend Over Time

Plot sales trends over weeks, months, and years.

Visualize sales by day or month using line plots.

Tren Penjualan Seiring Waktu

Memplot tren penjualan selama minggu, bulan, dan tahun.

Memvisualisasikan penjualan per hari atau bulan menggunakan grafik garis.

Top-Selling Products

Identify top-selling products by total revenue and units sold.

Create bar charts to visualize top categories and products.

Produk Terlaris

Mengidentifikasi produk terlaris berdasarkan total pendapatan dan unit yang terjual.

Membuat grafik batang untuk memvisualisasikan kategori dan produk teratas.

Customer Segmentation

Segment customers based on demographics such as age, location, or gender.

Perform group-by operations to understand customer preferences.

Segmentasi Pelanggan

Mensegmentasikan pelanggan berdasarkan demografi seperti umur, lokasi, atau jenis kelamin.

Melakukan operasi group-by untuk memahami preferensi pelanggan.

Geographical Analysis

Analyze customer locations and sales by region.

Visualize sales distribution across different cities or regions.

Analisis Geografis

Menganalisis lokasi pelanggan dan penjualan berdasarkan wilayah.

Memvisualisasikan distribusi penjualan di berbagai kota atau wilayah.

Customer Retention and Churn Analysis

Analyze repeat customers vs. one-time customers.

Investigate customer churn using retention rates.

Analisis Retensi dan Churn Pelanggan

Menganalisis pelanggan yang berulang vs. pelanggan satu kali.

Menyelidiki churn pelanggan menggunakan tingkat retensi.

Correlation Analysis

Examine relationships between numerical variables.

Use correlation heatmaps to visualize strong and weak correlations.

Analisis Korelasi

Memeriksa hubungan antara variabel numerik.

Menggunakan heatmap korelasi untuk memvisualisasikan korelasi yang kuat dan lemah.

Visualizations / Visualisasi
Sales Distribution by Product Line / Distribusi Penjualan Berdasarkan Kategori Produk:
KDE plot showing sales distribution across product lines.

python
Copy code
plt.figure(figsize=(10,6))
for product in data['Product line'].unique():
    subset = data[data['Product line'] == product]
    sns.kdeplot(subset['Total'], label=product)
plt.title('Distribution of Sales by Product Line')
plt.xlabel('Total Sales')
plt.ylabel('Density')
plt.legend()
plt.show()
Top 10 Selling Products / 10 Produk Terlaris:
Bar chart showing the top 10 best-selling products.

Sales Trends Over Time / Tren Penjualan Seiring Waktu:
Line plot to analyze sales trends over different time periods (daily, monthly, yearly).

Customer Age Distribution / Distribusi Usia Pelanggan:
Histogram to show the distribution of customer ages.

Geographical Sales Distribution / Distribusi Penjualan Geografis:
Map or bar chart showing sales by region.

Insights and Recommendations / Wawasan dan Rekomendasi
Top-selling products: The analysis shows that [Product A] and [Product B] are the most popular.

Sales trends: Sales peak during [specific time period], suggesting a focus on marketing during that time.

Customer segments: Customers in [specific region] tend to buy [specific product], indicating potential for targeted marketing.

Retention rates: A large portion of sales come from repeat customers, suggesting a need for customer loyalty programs.

Produk Terlaris: Analisis menunjukkan bahwa [Produk A] dan [Produk B] adalah yang paling populer.

Tren Penjualan: Penjualan mencapai puncak selama [periode waktu tertentu], menunjukkan fokus pada pemasaran selama waktu tersebut.

Segmen Pelanggan: Pelanggan di [wilayah tertentu] cenderung membeli [produk tertentu], menunjukkan potensi untuk pemasaran yang terarah.

Tingkat Retensi: Sebagian besar penjualan berasal dari pelanggan yang berulang, menunjukkan perlunya program loyalitas pelanggan.

Next Steps / Langkah Selanjutnya
Implement customer segmentation for targeted marketing.

Focus on regions with high sales potential based on demographic insights.

Create promotional strategies for low-selling products to increase overall revenue.

Implementasikan segmentasi pelanggan untuk pemasaran yang terarah.

Fokus pada wilayah dengan potensi penjualan tinggi berdasarkan wawasan demografi.

Buat strategi promosi untuk produk yang kurang laku untuk meningkatkan pendapatan keseluruhan.

How to Run the Project / Cara Menjalankan Proyek
Clone the repository:

bash
Copy code
git clone https://github.com/username/EDA-Sales-Analysis.git
Navigate to the project directory:

bash
Copy code
cd EDA-Sales-Analysis
Install the necessary dependencies (if required):

bash
Copy code
pip install -r requirements.txt
Open the Jupyter notebook and run the analysis:

bash
Copy code
jupyter notebook
Clone repositori:

bash
Copy code
git clone https://github.com/username/EDA-Sales-Analysis.git
Navigasi ke direktori proyek:

bash
Copy code
cd EDA-Sales-Analysis
Instal ketergantungan yang diperlukan (jika diperlukan):

bash
Copy code
pip install -r requirements.txt
Buka Jupyter notebook dan jalankan analisis:

bash
Copy code
jupyter notebook
Notes / Catatan
Dataset: The dataset used for this analysis can be found in the data/ folder.

Further Improvements: Future work may involve deeper analysis of customer lifetime value (CLV) and predictive modeling.

Dataset: Dataset yang digunakan untuk analisis ini dapat ditemukan di folder data/.

Perbaikan Lebih Lanjut: Pekerjaan mendatang dapat melibatkan analisis yang lebih mendalam tentang nilai umur pelanggan (CLV) dan pemodelan prediktif.
