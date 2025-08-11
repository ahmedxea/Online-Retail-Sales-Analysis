# 🛒 Online Retail Sales Analysis

This project analyzes sales data from a UK-based online retail store using **time series forecasting** and **customer segmentation**.  
The workflow combines Python for data preprocessing, visualization, and modeling with Power BI for interactive dashboarding.

---

## Dataset
- **Name:** [Online Retail II (UCI)](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci)  
- **Period:** 2009–2011  
- **Size:** 500,000+ transactional records  
- **Key fields:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country  

> **Note:** Due to GitHub file size limits, datasets are stored in a compressed file (`Data.zip`).  
> Unzip `Data.zip` and place its datasets in the same folder as the notebook before running the analysis.

---

## Project Pipeline
1. **Data Cleaning & Preprocessing**
   - Removed invalid transactions (zero price & refunds).
   - Converted dates to datetime format and created a `Revenue` column.
   - Engineered time-based features (Year, Month, Weekday, Hour, YearMonth).

2. **Exploratory Data Analysis (EDA)**
   - Sales trends over time.
   - Geographic and product-level breakdowns.
   - Customer purchasing patterns.

3. **Time Series Forecasting**
   - Checked stationarity using the Augmented Dickey-Fuller test.
   - Analyzed autocorrelation (ACF) & partial autocorrelation (PACF).
   - Compared **ARIMA** and **SARIMA** models for monthly revenue forecasting.

4. **Customer Segmentation**
   - Performed RFM (Recency, Frequency, Monetary) analysis.
   - Applied K-Means clustering on normalized RFM scores.
   - Grouped customers into segments for targeted business strategies.

5. **Visualization & Dashboard**
   - Created interactive Power BI dashboard with filters, slicers, and key metrics.
   - Added geographic sales maps, product rankings, and customer segments.
