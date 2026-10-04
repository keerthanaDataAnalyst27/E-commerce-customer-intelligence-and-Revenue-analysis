# E-commerce-customer-intelligence-and-Revenue-analysis
An end-to-end **E-Commerce Customer Intelligence and Revenue Analytics** project developed during a Data Analytics Internship.
The project uses Python to perform **data cleaning, exploratory data analysis, customer segmentation, statistical analysis, customer risk analysis, machine learning, and business insight generation**.

## 📌 Project Overview

This project analyzes e-commerce customer and order data to identify:

- Revenue and profit trends
- Category and product performance
- Customer purchasing behavior
- Customer segments using RFM analysis
- Repeat purchase behavior
- Customer churn/risk levels
- Acquisition-channel performance
- Discount and profit-margin relationships
- Order return patterns
- Machine-learning-based return prediction

## 🛠️ Technologies & Libraries

### Programming Language
- Python

### Libraries
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Scikit-learn
- Statsmodels

### Machine Learning
- Logistic Regression
- Random Forest Classifier
- Train/Test Split
- Stratified Cross-Validation
- Feature Preprocessing
- One-Hot Encoding
- Standard Scaling
- Model Evaluation

## 📂 Dataset Structure

The project works with an Excel-based e-commerce dataset containing sheets such as:

- `Customers`
- `Products`
- `Orders`
- `Monthly_Summary`
- `Category_Summary`

The raw data is preserved, while cleaning and transformations are performed on an analytical copy.

---

## 🔍 Project Workflow

### 1. Data Loading & Inspection

- Loaded multiple Excel sheets using Pandas
- Inspected dataset structure and dimensions
- Checked missing values
- Reviewed sample records

### 2. Data Cleaning

Performed:

- Duplicate order detection
- Duplicate removal
- Missing-value analysis
- Discount percentage treatment
- Delivery-day imputation
- Invalid-value checks
- Financial metric validation

The notebook identifies repeated order IDs and removes exact duplicate records while retaining legitimate repeated purchases.

---

## 💰 Revenue & Profit Analysis

Analyzed:

- Monthly revenue
- Monthly profit
- Number of orders
- Units sold
- Average Order Value (AOV)
- Month-over-month revenue growth
- Category revenue
- Category profit
- Profit margin
- Product-level performance

This helps identify high-revenue areas and categories/products where revenue is strong but margins require improvement.

---

## 👥 Customer Analytics

Customer-level analysis includes:

- Top customers by revenue
- Top customers by profit
- Customer order frequency
- Monetary value
- Recency
- Repeat purchase rate
- Average purchase gap
- Acquisition-channel analysis

---

## ⭐ RFM Customer Segmentation

RFM analysis was performed using:

- **Recency** — How recently a customer purchased
- **Frequency** — How frequently a customer purchased
- **Monetary** — How much revenue the customer generated

Customers were segmented into groups including:

- 🏆 Champions
- 💎 Loyal / Potential Loyalists
- ⚠️ At Risk
- 💤 Hibernating High Value
- 📌 Needs Attention

This segmentation can support targeted customer-retention strategies.

---

## ⚠️ Customer Risk Analysis

Customer-level risk features were created using:

- Recency
- Purchase frequency
- Monetary value
- Inactivity
- Low-frequency behavior
- Low monetary contribution

A customer **risk score** was calculated and customers were classified into:

- Low Risk
- Medium Risk
- High Risk
- Critical Risk

### Suggested retention strategies

| Risk Level | Suggested Action |
|---|---|
| Low | Loyalty programs & upselling |
| Medium | Customer nurturing |
| High | Targeted offers & reminders |
| Critical | Personalized win-back campaigns |

---

## 📈 Statistical Analysis

The project includes statistical analysis using SciPy and Statsmodels.

### Correlation Analysis

Spearman correlation was used to analyze relationships between:

- Quantity
- Discount %
- Delivery Days
- Net Sales
- Profit

### Hypothesis Testing

Two statistical tests were performed:

1. **Mann–Whitney U Test**
   - Compared profit distributions between returned and non-returned orders.

2. **Welch Independent-Samples T-Test**
   - Compared profit margins between high-discount and lower-discount orders.

---

## 🤖 Machine Learning

A classification model was developed to predict whether an order would be returned.

### Target

`return_flag`

### Features include

- Quantity
- Discount %
- Selling Price
- Payment Method
- Shipping Mode
- Category
- Age
- Gender
- Acquisition Channel
- Order Month

### Models Compared

#### Logistic Regression
A baseline classification model with class balancing.

#### Random Forest
An ensemble classification model using multiple decision trees.

### Evaluation Metrics

Because returned orders represent a relatively small proportion of the dataset, accuracy alone is not sufficient.

The models were evaluated using:

- Precision
- Recall
- F1 Score
- ROC-AUC
- Confusion Matrix
- Stratified Cross-Validation

---

## 📊 Data Visualizations

The project contains multiple visualizations, including:

1. Monthly Revenue
2. Revenue by Category
3. Profit Margin by Category
4. Returned vs Non-returned Orders
5. Order Value by Shipping Mode
6. Discount vs Profit Margin
7. Spearman Correlation Heatmap
8. Profit by Acquisition Channel

These visualizations help convert raw data into understandable business insights.

---

## 💡 Key Business Analysis Areas

The project identifies opportunities related to:

- Revenue growth
- Profit-margin improvement
- Discount optimization
- Product performance
- Customer retention
- Churn-risk management
- Return-risk prediction
- Acquisition-channel profitability
- Shipping performance
- Customer segmentation

---

## 🎯 Business Recommendations

Based on the analysis, potential actions include:

1. Improve pricing and discount strategies.
2. Monitor high-revenue categories with weak profit margins.
3. Create targeted campaigns for Champions.
4. Launch win-back campaigns for At-Risk customers.
5. Monitor Critical-risk customers closely.
6. Evaluate acquisition channels based on profitability, not only order volume.
7. Monitor products with high sales but low margins.
8. Use customer segmentation for personalized marketing.
9. Use return-risk predictions to improve operational planning.
10. Monitor discount levels to protect profit margins.

---

## 📁 Project Structure

```text
Ecommerce-Customer-Intelligence/
│
├── Ecommerce_Customer_Intelligence_Internship_Project.ipynb
├── README.md
│
└── dataset/
    └── ecommerce_internship_raw.xlsx
```

> **Note:** The raw Excel dataset is not included in this repository unless it is permitted to be publicly shared.

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### 2. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn statsmodels openpyxl
```

### 3. Open the notebook

```bash
jupyter notebook
```

Open:

```text
Ecommerce_Customer_Intelligence_Internship_Project.ipynb
```

### 4. Place the dataset

Keep the Excel dataset in the expected project location:

```text
ecommerce_internship_raw.xlsx
```

### 5. Run the notebook

Run the cells sequentially to reproduce the analysis.

---

## 🧠 Skills Demonstrated

This project demonstrates practical skills in:

- Python for Data Analytics
- Pandas
- NumPy
- Data Cleaning
- Exploratory Data Analysis
- Data Visualization
- Statistical Analysis
- Hypothesis Testing
- Customer Segmentation
- RFM Analysis
- Customer Risk Analysis
- Feature Engineering
- Machine Learning
- Classification
- Model Evaluation
- Cross-Validation
- Business Intelligence
- Business Insights
- Data-Driven Decision Making

---

## 👩‍💻 Project Type

**Data Analytics Internship Project**

**Domain:** E-Commerce / Customer Analytics

**Focus:** Revenue Analytics, Customer Intelligence & Predictive Analytics

**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn, Statsmodels

---

## 📌 Author

**Keerthana**

Data Analytics / Data Analyst Fresher

### Areas of Interest

- Data Analytics
- Business Intelligence
- Customer Analytics
- Python
- SQL
- Excel
- Power BI
- Machine Learning

