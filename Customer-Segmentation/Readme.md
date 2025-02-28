cat > README.md <<EOF
# 📌 Customer Segmentation in Retail Using RFM & K-Means Clustering

## **📖 Project Overview**
This project focuses on **customer segmentation** in the retail industry using **RFM (Recency, Frequency, Monetary) Analysis** and **K-Means Clustering**. By identifying different customer segments, businesses can optimize marketing strategies, enhance customer retention, and personalize offers for better engagement and profitability.

## **🛠️ Tech Stack**
- **Programming Language**: Python 🐍
- **Data Processing**: Pandas, NumPy
- **Clustering Algorithms**: K-Means, DBSCAN, Hierarchical Clustering
- **Machine Learning & Evaluation**: Scikit-learn
- **Time Series Forecasting**: Prophet (for demand forecasting)
- **Visualization**: Matplotlib, Seaborn
- **Development Environment**: Jupyter Notebook / Google Colab




<img Src="Customer-Segmentation/Reports/Images/download (1).png" >


---

## **📌 Project Workflow**
### **1️⃣ Data Collection & Preprocessing**
- **Dataset Used**: Online Retail Dataset
- **Key Columns Used**:
  - \`CustomerID\`: Unique customer identifier
  - \`InvoiceDate\`: Purchase date
  - \`InvoiceNo\`: Unique transaction number
  - \`Quantity\`: Number of items purchased
  - \`UnitPrice\`: Price per unit
  - \`TotalPrice\`: Derived as \`Quantity * UnitPrice\`

### **2️⃣ Feature Engineering**
- **RFM Calculation**:
  - \`Recency (R)\`: Days since last purchase
  - \`Frequency (F)\`: Number of transactions
  - \`Monetary (M)\`: Total amount spent
- **Handling Missing Values & Outliers**:
  - Removed negative transactions (returns)
  - Handled missing \`CustomerID\` values
  - Used **IQR Method** for outlier detection

### **3️⃣ Customer Segmentation Using K-Means**
- **Scaling Data** using \`StandardScaler\`
- **Finding Optimal Clusters (K) using Silhouette Score**
- **Applying K-Means Algorithm**
- **Visualizing Segments using Pairplots & Cluster Heatmaps**

### **4️⃣ Advanced Evaluation Metrics**
- **Silhouette Score** – Measures how well-separated the clusters are
- **Davies-Bouldin Index** – Evaluates cluster compactness and separation
- **Calinski-Harabasz Score** – Assesses intra-cluster density and inter-cluster separation

### **5️⃣ Demand Forecasting (Optional)**
- Used **Prophet** for predicting future sales
- Generated a **30-day sales forecast** to assist in demand planning

---

## **📌 Key Results & Findings**
✅ Customers are segmented into different groups such as **loyal customers, frequent buyers, and inactive users**.  
✅ **Silhouette Score (0.602):** Indicates good cluster separation.  
✅ **Sales Forecasting** provides valuable insights for predicting demand trends and optimizing inventory.  

---

## **📌 How to Run the Project**
1️⃣ Install dependencies:
\`\`\`bash
pip install pandas numpy scikit-learn matplotlib seaborn prophet
\`\`\`
2️⃣ Run the script:
\`\`\`bash
python customer_segmentation.py
\`\`\`

EOF
