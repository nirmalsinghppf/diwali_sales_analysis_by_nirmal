# 🪔 Diwali Sales Analysis

Exploratory Data Analysis (EDA) of Diwali sales data to understand customer demographics and buying behavior using Python, Pandas, and Seaborn/Matplotlib.

## 📌 Overview

This project analyzes a retail dataset of **11,251 transactions** collected during the Diwali sales season in India. The goal is to uncover patterns in *who* is buying, *what* they're buying, and *how much* they're spending — segmented by gender, age, location, marital status, and occupation.

## 📂 Dataset

The dataset (`Diwali Sales Data.csv`) contains 15 columns including:

| Column | Description |
|---|---|
| `User_ID`, `Cust_name` | Customer identifiers |
| `Product_ID`, `Product_Category` | Product details |
| `Gender`, `Age Group`, `Age` | Customer demographics |
| `Marital_Status` | 0 = Unmarried, 1 = Married |
| `State`, `Zone` | Customer location |
| `Occupation` | Customer's profession |
| `Orders`, `Amount` | Purchase quantity and value |

*(Two blank columns, `Status` and `unnamed1`, are dropped during cleaning.)*

## 🧹 Data Cleaning

- Dropped fully empty/unrelated columns (`Status`, `unnamed1`)
- Removed rows with null values (in `Amount`)
- Corrected data types (e.g., `Amount` cast to `int`)
- Renamed columns for clarity

## 📊 Exploratory Data Analysis

The analysis explores sales patterns across:

- **Gender** — purchase count and total amount spent by gender
- **Age Group** — buyer distribution across age brackets, split by gender
- **State** — top 10 states by order volume and total sales
- **Marital Status** — spending patterns of married vs. unmarried customers
- **Occupation** — sales by customer profession
- **Product Category** — best-selling product categories
- **Top Products** — top 10 best-selling products by order count

## 🔑 Key Findings

- Most buyers are **female**, and women also show **higher purchasing power** than men.
- The largest buyer segment is **women aged 26–35**.
- **Uttar Pradesh, Maharashtra, and Karnataka** lead in both order volume and total sales.
- **Married women** make up the biggest-spending group.
- Buyers are concentrated in the **IT, Healthcare, and Aviation** sectors.
- **Food, Clothing, and Electronics** are the top-selling product categories.

**Conclusion:** Married women aged 26–35 from UP, Maharashtra, and Karnataka, working in IT, Healthcare, and Aviation, are the most likely to purchase Food, Clothing, and Electronics products.

## 🛠️ Tech Stack

- Python 3
- Pandas & NumPy — data manipulation
- Matplotlib & Seaborn — data visualization
- Jupyter Notebook

## 🚀 Getting Started

```bash
git clone https://github.com/<your-username>/diwali-sales-analysis.git
cd diwali-sales-analysis
pip install -r requirements.txt
jupyter notebook Diwali_Sales_Analysis.ipynb
```

### Requirements

```
pandas
numpy
matplotlib
seaborn
jupyter
```

## 📁 Project Structure

```
├── Diwali_Sales_Analysis.ipynb   # Main analysis notebook
├── Diwali Sales Data.csv         # Raw dataset
└── README.md
```

## 📈 Future Improvements

- Build an interactive dashboard (e.g., Power BI / Streamlit)
- Add predictive modeling for customer spend
- Deeper zone-wise and category-wise cross analysis

## 📝 License

This project is open source and available for learning purposes.
