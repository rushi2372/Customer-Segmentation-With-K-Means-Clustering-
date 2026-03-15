# 🛍️ Customer Segmentation with K-Means Clustering

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-1.3%2B-orange?logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

## 📌 Overview

This project applies **K-Means Clustering** — an unsupervised machine learning algorithm — to segment mall customers based on their **Annual Income** and **Spending Score**.

By identifying distinct customer groups, businesses can craft **targeted marketing strategies** that improve customer engagement and overall satisfaction.

---

## 📁 Project Structure

```
customer-segmentation/
│
├── data/
│   └── Mall_Customers.csv          # Raw dataset
│
├── notebooks/
│   └── Customer_Segmentation_KMeans.ipynb  # Main analysis notebook
│
├── images/
│   ├── eda_distributions.png       # EDA plots (auto-generated)
│   ├── gender_distribution.png     # Gender pie chart (auto-generated)
│   ├── elbow_method.png            # Elbow curve (auto-generated)
│   └── customer_clusters.png       # Final cluster visualization (auto-generated)
│
├── requirements.txt                # Python dependencies
├── .gitignore
└── README.md
```

---

## 📊 Dataset

**Source:** [Kaggle — Mall Customer Segmentation Data](https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python)

| Feature | Description |
|---|---|
| `CustomerID` | Unique identifier for each customer |
| `Gender` | Male / Female |
| `Age` | Age of the customer |
| `Annual Income (k$)` | Annual income in thousands of USD |
| `Spending Score (1-100)` | Score assigned based on customer spending behavior |

- **Rows:** 200 customers  
- **No missing values**

---

## 🔄 Workflow

```
Load Data → EDA → Preprocessing → Elbow Method → K-Means Training → Visualization → Insights
```

1. **Load & Explore** — Load the dataset and perform basic EDA
2. **Preprocess** — Check for nulls and select clustering features
3. **Elbow Method** — Determine optimal number of clusters (k = 5)
4. **Train Model** — Fit K-Means with `k-means++` initialization
5. **Visualize** — Plot customer segments with centroids
6. **Insights** — Derive actionable marketing strategies per cluster

---

## 📈 Results

### Elbow Method
The WCSS elbow appears clearly at **k = 5**, confirming 5 optimal clusters.

### Customer Segments

| Cluster | Profile | Recommended Strategy |
|---|---|---|
| 🟢 Cluster 1 | Low Income, Low Spend | Budget deals, value promotions |
| 🔴 Cluster 2 | High Income, Low Spend | Premium product showcases, personalized offers |
| 🟡 Cluster 3 | Mid Income, Mid Spend | Membership programs, seasonal campaigns |
| 🟣 Cluster 4 | Low Income, High Spend | Loyalty rewards, early-access deals |
| 🔵 Cluster 5 | High Income, High Spend | VIP programs, luxury product lines |

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/customer-segmentation.git
cd customer-segmentation
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Launch Jupyter Notebook

```bash
jupyter notebook notebooks/Customer_Segmentation_KMeans.ipynb
```

---

## 🧰 Tech Stack

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical operations |
| `matplotlib` | Plotting and visualization |
| `seaborn` | Enhanced statistical plots |
| `scikit-learn` | K-Means clustering algorithm |

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙋 Author

Feel free to reach out for any questions or suggestions!

- **Name:** **Rushikesh Sangamnere**
- **Email:**  **rushikeshsangamnere4561@gmail.com**
- **Phone:**  **+91 9096506345**
