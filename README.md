# E-Commerce Sales Data Analysis

## Objective
The main objective of this project is to analyze an e-commerce sales dataset to uncover insights and trends, such as:
- **Sales performance over time**: Understanding the sales trends to make data-driven decisions for the business.
- **Best-selling products**: Identifying the top-performing products in terms of sales.
- **Customer demographics**: Analyzing customer data to understand which demographics are contributing the most to sales.
- **Customer retention**: Analyzing customer retention rates and recommending strategies for improvement.

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

# E-Commerce Sales Analysis

## Objective
The main objective of this project is to analyze an e-commerce sales dataset to uncover insights and trends, including:
- **Sales Performance Over Time**: Understanding the sales trends to drive data-based decisions for business improvements.
- **Best-Selling Products**: Identifying top-performing products based on total revenue and units sold.
- **Customer Demographics**: Analyzing customer demographics such as age, location, or gender to identify key segments contributing to sales.
- **Customer Retention**: Analyzing customer retention rates and providing strategies to improve customer loyalty.

## Steps of Exploratory Data Analysis (EDA)

### 1. Data Cleaning
   - Remove or handle missing data.
   - Convert data types (e.g., date formatting).
   - Handle outliers and incorrect values.

### 2. Understanding the Data
   - Get an overview of the dataset (e.g., data types, number of rows, columns).
   - Summarize the dataset using functions like `df.describe()` and `df.info()`.

### 3. Univariate Analysis
   - Analyze individual columns or features.
   - Example: Distribution of sales in different product categories.

### 4. Multivariate Analysis
   - Examine relationships between two or more variables.
   - Example: Comparing sales amount versus customer age.

### 5. Sales Trend Over Time
   - Plot sales trends over weeks, months, and years using line plots.

### 6. Top-Selling Products
   - Identify top-selling products by total revenue and units sold.
   - Create bar charts to visualize top categories and products.

### 7. Customer Segmentation
   - Segment customers based on demographics like age, location, or gender.
   - Perform group-by operations to understand customer preferences.

### 8. Geographical Analysis
   - Analyze customer locations and sales by region.
   - Visualize sales distribution across cities or regions.

### 9. Customer Retention and Churn Analysis
   - Analyze repeat customers versus one-time customers.
   - Investigate churn using retention rates.

### 10. Correlation Analysis
   - Examine relationships between numerical variables.
   - Visualize strong and weak correlations using heatmaps.

## Tools Used
- **Python**: 
  - **Pandas**: For data manipulation and analysis.
  - **Matplotlib**: For data visualization.
  - **Seaborn**: For statistical data visualization.
- **Jupyter Notebook**: For writing code and visualizing results interactively.
- **Git**: For version control and project collaboration.
- **GitHub**: For hosting the project repository.

:



Visualizations / Visualisasi
Sales Distribution by Product Line / Distribusi Penjualan Berdasarkan Kategori Produk:
KDE plot showing sales distribution across product lines.
``` bash
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
```

``` bash
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
jupyter notebook
Notes / Catatan
Dataset: The dataset used for this analysis can be found in the data/ folder.

Further Improvements: Future work may involve deeper analysis of customer lifetime value (CLV) and predictive modeling.

Dataset: Dataset yang digunakan untuk analisis ini dapat ditemukan di folder data/.

Perbaikan Lebih Lanjut: Pekerjaan mendatang dapat melibatkan analisis yang lebih mendalam tentang nilai umur pelanggan (CLV) dan pemodelan prediktif.
```