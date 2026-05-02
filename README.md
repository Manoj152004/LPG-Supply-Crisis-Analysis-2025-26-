# LPG Supply Crisis Analysis (2025–2026)

## 📌 Project Overview

This project analyzes the impact of an LPG supply crisis using a large-scale dataset (~200K+ rows, 11 fields). Since real-world granular data was not publicly available, a synthetic (dummy) dataset was generated and then processed to simulate realistic demand, supply, and pricing behavior.

**The objective is to:**
- Identify supply-demand gaps
- Analyze price fluctuations during crisis periods
- Detect state-wise impact

---

## 📊 Dataset Information

| Attribute | Details |
|-----------|---------|
| Total Rows (after cleaning) | ~204,270 |
| Columns | Date, State, Demand_MT, Supply_MT, Imports_MT, Crisis_Flag, Price_INR, Gap_MT |

---

## ⚙️ Data Pipeline

### 1. Data Loading
- Dataset loaded using CSV reader
- Shape and columns inspected

### 2. Initial Data Checks
- Dataset size and structure verified
- Missing values identified
- Duplicate records detected

### 3. Data Cleaning

**🔹 Remove Duplicates**
- Duplicate rows removed from dataset

**🔹 Handle Missing Values**
- Forward fill used for time-series consistency on Demand and Price columns

**🔹 Fix Data Types**
- Date column converted to datetime format
- Price column converted to numeric type

**🔹 Handle Outliers**
- Extreme values (e.g., 9999) treated as null and imputed with median values

**🔹 Feature Engineering**
- Gap_MT calculated as Demand minus Supply
- Time extracted from Date column

---

## 📈 Tableau Dashboard

The cleaned dataset was visualized using Tableau.

**🔹 Key Visuals**

1. **Demand vs Supply Trend** — Shows stable demand vs declining supply during crisis
2. **Price Trend** — Highlights price spike during supply shortage
3. **Crisis vs Normal Comparison** — Average supply drops significantly in crisis period
4. **Top 5 States by Gap** — Identifies most affected regions
5. **Demand by State** — Shows highest consumption regions

---

## 🔍 Key Insights

- Supply dropped significantly during crisis periods
- Demand remained relatively stable → caused imbalance
- Prices increased sharply due to supply shortage
- High-demand states (e.g., Uttar Pradesh, Bihar) faced the largest gaps
- Crisis impact was uneven across regions

---

## 🧠 Conclusion

This project demonstrates how supply chain disruptions directly affect pricing and availability. The analysis highlights the importance of:

- Efficient distribution systems
- Supply stabilization strategies
- Regional demand planning

---

## 🤖 Use of AI

- AI was used to:
  - Generate synthetic dataset
  - Assist in data preprocessing logic
  - Guide visualization and analysis

- Final implementation, logic, and interpretation were done manually.

---

## 🚀 Tools Used

- Python (Pandas, NumPy)
- Tableau
- GitHub

---

## 📁 Project Workflow

1. Generate synthetic dataset
2. Clean and preprocess data (Python)
3. Perform analysis
4. Build dashboard (Tableau)
5. Extract insights

---

## 📌 Final Note

This is a portfolio project designed to demonstrate:
- Data cleaning skills
- Analytical thinking
- Visualization ability
- End-to-end data workflow

---

## 📷 Dashboard Preview
<img width="1366" height="768" alt="Screenshot (145)" src="https://github.com/user-attachments/assets/efae017c-4e2f-4eb1-96ed-3704ae36ae0e" />

## 🔗 Author 
#Manoj


**Data Analyst Project**

**Email:** *(ak9190959@gmail.com)*

---

## 📄 License

This project is for portfolio and educational purposes only.
