# Customer Segmentation Using K-Means Clustering

## Project Overview
This project focuses on segmenting customers based on their purchasing behavior using **K-Means Clustering**. The analysis aims to uncover actionable insights that businesses can leverage for **targeted marketing** and **improved customer engagement**. Dimensionality reduction techniques like **Principal Component Analysis (PCA)** are utilized to optimize the dataset while preserving key variance.

---

## Objectives
- Identify meaningful customer groups based on transaction patterns.
- Optimize clustering by reducing dataset dimensionality using PCA.
- Provide actionable insights to enhance business strategies, including personalized marketing and customer retention.

---

## Dataset Details
- **Source**: Retail transactional data.
- **Features**:
  - `InvoiceNo`: Transaction identifier.
  - `StockCode`: Product identifier.
  - `Description`: Product description.
  - `Quantity`: Number of items purchased.
  - `InvoiceDate`: Transaction date and time.
  - `UnitPrice`: Price per item.
  - `CustomerID`: Unique customer identifier.
  - `Country`: Country of transaction.
- **Size**: 4,067 records after preprocessing.

---

## Key Steps
1. **Data Cleaning**:
   - Removed duplicates and rows with missing critical fields.
   - Filtered out non-product transactions (e.g., "POST", "BANK CHARGES").
   - Identified and excluded outliers using the Isolation Forest algorithm.

2. **Feature Engineering**:
   - Generated features like `Total Spend`, `Average Transaction Value`, `Cancellation Rate`, and `Days Since Last Purchase`.

3. **Dimensionality Reduction**:
   - Applied PCA to reduce dimensions while retaining **96% variance**.
   - Reduced dataset to 6 principal components.

4. **Clustering Methodology**:
   - Used **K-Means** to segment customers into clusters.
   - Optimal number of clusters (`k=3`) determined using the Elbow Method and Silhouette Analysis.

5. **Evaluation**:
   - Metrics used: Silhouette Score (0.23), Calinski-Harabasz Score (1216.78), Davies-Bouldin Score (1.41).
   - Validated cluster quality with radar charts and 3D scatter plots.

---

## Results and Insights
- **Cluster Profiles**:
  - **Cluster 0**: High-value, frequent shoppers (17.92% of customers).
  - **Cluster 1**: Low-value, disengaged customers (40.82% of customers).
  - **Cluster 2**: Moderate-value, steady shoppers (41.26% of customers).
- **Actionable Recommendations**:
  - Focus on retaining high-value customers (Cluster 0) with loyalty programs.
  - Re-engage disengaged customers (Cluster 1) with targeted campaigns.
  - Maintain steady engagement with average customers (Cluster 2) through personalized promotions.

---


