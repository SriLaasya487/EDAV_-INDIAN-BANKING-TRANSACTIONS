# 🏦 Indian Banking Transactions – Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) on an Indian Banking Transactions dataset containing **550,000 transactions across 20 columns**, covering the period from January 2019 to January 2024.

The objective is to explore banking transaction patterns, identify factors associated with fraudulent activities, analyse transaction failures, and understand customer behaviour using Python's data analysis and visualization libraries.

The project follows a complete EDA workflow, from data understanding and preprocessing to statistical analysis, time-series exploration, and visualization.

## 🎯 Objectives

The analysis aims to answer five key questions:

1. **Transaction Value Analysis:** Which transaction types, banking channels, states, and merchant categories contribute the most to transaction value?
2. **Time-Series Analysis:** How do banking transactions change over time, across months, quarters, years, hours, and weekdays?
3. **Fraud Analysis:** Is fraudulent activity associated with transaction amount, channel, time, KYC status, credit score, or transaction type?
4. **Transaction Failure Analysis:** How frequently do transactions fail, and are failures concentrated in particular channels or transaction types?
5. **Customer Analysis:** What patterns can be identified in customer credit ratings, loans, account balances, and transaction behaviour?

## 🛠️ Technologies & Libraries Used

| Technology | Purpose |
|---|---|
| Python | Programming language |
| NumPy | Numerical operations and data manipulation |
| Pandas | Data cleaning, transformation, aggregation and analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Google Colab / Jupyter Notebook | Development environment |

## 📂 Project Structure

```text
Indian-Banking-Transactions-EDA/
│
├── indian_banking_transactions_project.ipynb
│
├── indian_banking_transactions.csv
│
└── README.md
```

## 🔍 Project Workflow

### 1. Data Loading & Understanding
- Imported the required Python libraries.
- Loaded the banking transactions dataset using Pandas.
- Examined dataset dimensions, column names, data types and index.
- Used descriptive statistics to understand numerical and categorical variables.
- Identified unique values and transaction distributions.

### 2. Data Cleaning & Preprocessing
- Identified missing values and handled missing loan information.
- Replaced inconsistent labels and improved readability.
- Converted date columns into appropriate datetime formats.
- Optimized categorical and numerical data types.
- Detected and removed duplicate transaction IDs.
- Performed basic data validation and checked for unusual values.

### 3. Data Transformation & Categorization
- Used mapping and renaming operations to improve data readability.
- Applied `pd.cut()` to categorize credit scores, transaction amounts and time periods.
- Used `pd.qcut()` to create transaction amount tiers.
- Performed sorting and conditional filtering to identify specific transaction patterns.

### 4. Hierarchical Indexing & Data Reshaping
- Implemented multi-level indexing using `set_index()`.
- Explored data concatenation.
- Used `stack()` and `unstack()` to reshape data.
- Applied `pivot()` and `pivot_table()` for multidimensional analysis.

### 5. GroupBy & Time-Series Analysis
- Grouped transactions by different categorical variables.
- Applied aggregation functions such as `sum()`, `mean()`, `count()` and `median()`.
- Converted transaction timestamps into a DatetimeIndex.
- Performed date-based filtering and selection.
- Used `resample()` for monthly, quarterly and yearly analysis.
- Explored seasonality, weekday patterns and hourly transaction activity.

### 6. Exploratory Data Analysis & Visualization

The project includes five major analytical sections:

- Transaction type, channel, state and merchant category analysis.
- Monthly, quarterly and yearly transaction trends.
- Fraud distribution and its relationship with transaction characteristics.
- Transaction success, failure, pending and reversal analysis.
- Customer credit ratings, loan distribution and account balance analysis.

Visualizations include:
- Bar charts
- Line charts
- Histograms
- Pie charts
- Heatmaps
- Time-series plots
- Moving averages and trend lines

## 📊 Key Findings & Insights

### 1. Transaction Value
- Total transaction value is approximately **₹1,645 crore**.
- RTGS contributes approximately **54% of the total transaction value**.
- UPI accounts for approximately **28% of transactions**, but only 1.3% of total value.
- Maharashtra, Karnataka, Tamil Nadu and Delhi together contribute approximately 57% of transaction value.
- Approximately 10% of transactions account for 85% of the total value.

### 2. Transaction Trends
- Transaction activity remains relatively stable between 2019 and 2023.
- Each year records approximately 110,000 transactions.
- No statistically significant long-term growth trend was identified.
- No strong seasonal or hourly transaction pattern was observed.

### 3. Fraud Analysis
- Overall fraud rate is approximately **0.89%** (4,873 transactions).
- Fraudulent transactions account for approximately ₹58 crore.
- Transaction amount is a major factor associated with fraud.
- Transactions of ₹5 lakh and above show a substantially higher fraud rate.
- Channel, KYC status, credit score and hour of transaction do not show meaningful differences in fraud rates in this dataset.

### 4. Transaction Failures
- Approximately 92% of transactions are successful.
- Around 4% of transactions fail.
- The remaining transactions are reversed or pending.
- Failure rates are relatively consistent across different channels and transaction types.

### 5. Customer Behaviour
- The dataset contains approximately 79,916 distinct customer IDs.
- Around 35% of transactions are associated with customers having loans.
- Personal loans are the most common loan category.
- The median account balance is approximately ₹36,400, compared with a mean of approximately ₹84,600.
- The top 10% of customers contribute approximately 50% of transaction value.

## 💡 Conclusion

This project demonstrates how exploratory data analysis can uncover meaningful patterns in large-scale banking transaction data.

The analysis highlights the differences between transaction frequency and transaction value, explores temporal patterns, examines fraud-related characteristics, and evaluates transaction reliability and customer behaviour.

An important finding is that transaction amount is more informative for identifying elevated fraud rates than several commonly examined categorical characteristics.

Overall, the project demonstrates the application of Python-based data analysis techniques to investigate financial data and communicate insights through statistical summaries and visualizations.

## 🚀 How to Run the Project

**Option 1: Google Colab**

1. Download the Jupyter Notebook.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the `.ipynb` file.
4. Upload `indian_banking_transactions.csv` when prompted by the notebook.
5. Run all cells sequentially.

**Option 2: Jupyter Notebook (Local Environment)**

1. Clone the repository:

```bash
git clone https://github.com/your-username/Indian-Banking-Transactions-EDA.git
```

2. Navigate to the project directory:

```bash
cd Indian-Banking-Transactions-EDA
```

3. Install the required libraries:

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

4. Launch Jupyter Notebook:

```bash
jupyter notebook
```

5. Open the notebook and execute the cells.

**Note:** The CSV dataset must be placed in the project directory. The notebook currently uses Google Colab's file-upload functionality, so the data-loading cell may need to be adjusted when running locally.

## 📁 Dataset Information

| Attribute | Details |
|---|---|
| Dataset | Indian Banking Transactions |
| Records | 550,000 |
| Features | 20 columns |
| Time Period | January 2019 – January 2024 |
| Domain | Banking and Financial Analytics |
| Format | CSV |

The dataset file is required separately to reproduce the analysis.

## 👩‍💻 Project Type

**End-to-End Exploratory Data Analysis (EDA)**

**Domain:** Banking & Financial Analytics

**Focus Areas:** Data Cleaning, Data Wrangling, Statistical Analysis, GroupBy Operations, Hierarchical Indexing, Time-Series Analysis, Fraud Analysis and Data Visualization.

---

*If you found this project interesting, feel free to explore the notebook and its visualizations!* ⭐
