# Customer Churn Prediction Using Classification Models and Text Mining in Retail Data Warehousing

> A Text Mining and Data Mining project that predicts customer churn in retail using RFM analysis, classification models, and NLP techniques.

---

## 👩‍💻 Authors

- **Sri Varshini S** — srivarshini.s2022@vitstudent.ac.in
- **Rakhi Mol V** — rakhimol.v@vit.ac.in

---

## 📌 Project Overview

Customer churn — when customers stop purchasing from a retailer — is a major threat to business profitability. This project uses the **Online Retail Dataset** to build a churn prediction pipeline that combines:

- RFM Feature Engineering (Recency, Frequency, Monetary)
- Classification Models (Logistic Regression, Decision Tree, Random Forest, SVM)
- Text Mining (TF-IDF, Word Cloud on product descriptions)
- Evaluation Metrics (Accuracy, Precision, Recall, F1-Score, ROC-AUC)

---

## 📂 Project Structure

```
├── report.docx                  # Full case study report
├── churn_prediction.ipynb       # Jupyter Notebook implementation
├── dataset/
│   └── online_retail.csv        # Online Retail Dataset (CSV)
├── outputs/
│   ├── wordcloud.png            # Word Cloud of product descriptions
│   ├── confusion_matrix.png     # Confusion Matrix
│   ├── roc_curve.png            # ROC Curve comparison
│   └── feature_importance.png   # Random Forest feature importance
└── README.md
```

---

## 📊 Dataset

**Online Retail Dataset** — transactional data from a UK-based retailer.

| Column | Description |
|---|---|
| Invoice | Invoice number |
| StockCode | Product code |
| Description | Product name (used for Text Mining) |
| Quantity | Number of units purchased |
| InvoiceDate | Date and time of purchase |
| Price | Unit price |
| Customer ID | Unique customer identifier |
| Country | Country of the customer |

> Dataset source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/online+retail) or Kaggle

---

## 🛠️ Requirements

Install all dependencies using:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn wordcloud nltk xgboost
```

Or inside Jupyter Notebook:

```python
import sys
!{sys.executable} -m pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn wordcloud nltk xgboost
```

| Library | Purpose |
|---|---|
| pandas | Data loading and manipulation |
| numpy | Numerical computations |
| scikit-learn | ML models and evaluation |
| matplotlib | Plotting graphs |
| seaborn | Data visualization |
| imbalanced-learn | SMOTE for class imbalance |
| wordcloud | Word Cloud generation |
| nltk | Text preprocessing |
| xgboost | Gradient boosting model |

---

## 🚀 How to Run

1. **Clone or download** this repository
2. **Place the dataset** (`online_retail.csv`) in the `dataset/` folder
3. **Open Jupyter Notebook**
   ```bash
   jupyter notebook
   ```
4. **Open** `churn_prediction.ipynb`
5. **Run all cells** in order (Cell → Run All)

---

## ⚙️ Implementation Steps

| Step | Description |
|---|---|
| 1 | Load and explore the dataset |
| 2 | Clean data (remove nulls, cancelled invoices, negative values) |
| 3 | Engineer RFM features (Recency, Frequency, Monetary) |
| 4 | Label churn (Recency ≥ 90 days = Churned) |
| 5 | Train classification models |
| 6 | Handle class imbalance using SMOTE |
| 7 | Evaluate using Accuracy, F1, ROC-AUC |
| 8 | Apply TF-IDF and Word Cloud on Description column |
| 9 | Plot Confusion Matrix and Feature Importance |

---

## 📈 Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

---

## 🔑 Key Results

- **Random Forest** achieved the best overall performance
- **TF-IDF** on product descriptions revealed top purchased categories
- **SMOTE** improved recall for minority churn class
- **RFM features** — Recency was the most important predictor of churn

---

## 📚 References

1. Zaghloul, M., Barakat, S., & Rezk, A. (2025). Enhancing customer retention in Online Retail through churn prediction: A hybrid RFM, K-means, and deep neural network approach. *Expert Systems with Applications*, 290, 128465.
2. Javaherihaghighi, S., & Oloruntoba, O. Advanced Database Management and Data Mining for optimizing supervised e-commerce customers behavior prediction.
3. Tiwari, P. P., Yuktha, G. P., & Manimaran, A. (2025). Utilizing Business Intelligence and Machine Learning in CRM Data to Reduce Customer Churn in E-commerce Platforms. IGI Global.
4. Clinton, P. B., et al. (2025). Machine Learning on Retail Stores for Customer Churn. ICoACT 2025, IEEE.
5. Ehsani, F., & Hosseini, M. (2025). Customer churn analysis using feature optimization methods and tree-based classifiers. *Journal of Services Marketing*, 39(1), 20–35.
6. Barzegar, M., & Hasani, A. (2024). Analyzing customer churn behavior using data mining approach. *International Journal of Research in Industrial Engineering*, 13(4), 384–398.
7. Aaron, J., et al. (2024). The Use of Churn-Prediction to Improve Customer-Retention in Grocery E-Retailing. CRC Press.

---

## 🏫 Course

**Data Warehouse and Data Mining / Text Mining**
Vellore Institute of Technology (VIT)
