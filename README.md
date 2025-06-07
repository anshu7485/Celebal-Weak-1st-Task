# 🧠 Customer Lifetime Value Prediction (CLV)

This project focuses on predicting the **Customer Lifetime Value (CLV)** using online retail data. We use historical purchase behavior to estimate the future value of a customer for a business over their entire relationship.

## 📁 Dataset

- **Source**: [Online Retail Dataset - Kaggle](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset)
- **Records**: 541,910 transactions
- **Columns**: InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country

---

## 🎯 Objective

To build a machine learning model that predicts **Customer Lifetime Value (CLV)** by incorporating:
- Past purchase history
- Purchase frequency
- Recency and tenure
- Total quantity and order behavior

---

## 🔍 Features Engineered

| Feature          | Description |
|------------------|-------------|
| `Recency`        | Days since last purchase |
| `Tenure`         | Days between first and last purchase |
| `Frequency`      | Number of unique invoices |
| `Monetary`       | Total amount spent |
| `TotalQuantity`  | Total number of items purchased |
| `AvgOrderValue`  | Average value per order |
| `CLV`            | Target: total value spent by customer |

---

## 🤖 Models Used

| Model              | R² Score | RMSE (log / real) |
|--------------------|----------|-------------------|
| Linear Regression  | 0.63     | 0.77 (log scale)  |
| 🔥 XGBoost         | **0.86** | **3755.18 (real)** |

👉 Final model: **XGBoost + log-transformed CLV**

---

## 📷 Sample Visualization

![CLV Distribution](https://github.com/anshu7485/Celebal-Weak-1st-Task/blob/main/output.png)  

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/clv-prediction.git
   cd clv-prediction
