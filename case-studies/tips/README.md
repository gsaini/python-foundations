# 🍽️ Tips Case Study

A comprehensive data analysis project exploring tipping patterns at Chef's Kitchen restaurant in San Diego. This case study uses Python data analysis and visualization techniques to uncover insights about customer behavior, billing patterns, and tipping habits across different demographics.

---

## 📋 Table of Contents

- [Context](#context)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Key Analysis Steps](#key-analysis-steps)
- [Key Insights & Findings](#key-insights--findings)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)

---

## 🎯 Context

A **tip** is a monetary incentive given by customers or guests for polite, prompt, and efficient service provided by the staff. The practice of giving tips has been continuing for a very long time and has become particularly popular in service industries such as hotels and restaurants.

Understanding tipping patterns helps restaurant management:

- Motivate staff through performance-based incentives
- Identify high-revenue periods and customer segments
- Optimize staffing decisions
- Improve customer service strategies

---

## 🎯 Objective

**Chef's Kitchen** is one of the most popular restaurants in the city of San Diego and acts as a one-stop destination for food lovers. The polite and efficient service provided by the restaurant staff often gets them tips from customers.

As a **Data Analyst** for the restaurant, the task is to:

1. Analyze the provided data to identify patterns and trends in revenue and tips
2. Explore tipping behavior across different customer demographics
3. Create informative visualizations to convey insights
4. Provide actionable recommendations based on the analysis

---

## 📊 Dataset Description

The dataset contains **244 records** with the following **8 features**:

| Feature      | Description                                                  | Data Type   |
| ------------ | ------------------------------------------------------------ | ----------- |
| `order_id`   | Unique identifier of each order                              | Integer     |
| `day`        | Day of the week when the customer visited (Thur/Fri/Sat/Sun) | Categorical |
| `time`       | Time of day when the customer visited (Lunch/Dinner)         | Categorical |
| `size`       | Number of people present at the table (1-6)                  | Integer     |
| `smoker`     | Whether the table included smokers (Yes/No)                  | Categorical |
| `sex`        | Gender of the bill payer (Male/Female)                       | Categorical |
| `total_bill` | The bill amount in dollars ($3.07 - $50.81)                  | Float       |
| `tip`        | The tip amount in dollars ($1 - $10)                         | Float       |

### Key Statistics:

- **Bill Amount**: Ranges from ~$3 to ~$51, with an average of ~$20
- **Tip Amount**: Ranges from ~$1 to ~$10, with an average of ~$3
- **Group Size**: Varies from 1 to 6 people

---

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computations
- **Matplotlib** - Basic plotting and visualization
- **Seaborn** - Statistical data visualization

---

## 📁 Project Structure

```
tips/
├── README.md                    # Project documentation (this file)
├── Tips_Case_Study.ipynb        # Jupyter notebook with complete analysis
└── tips.csv                     # Dataset file
```

---

## 🔍 Key Analysis Steps

### 1. Data Loading & Preprocessing

- Import necessary libraries (pandas, numpy, matplotlib, seaborn)
- Load the dataset from CSV
- Drop unnecessary columns (`order_id`)
- Verify data types and check for missing values

### 2. Exploratory Data Analysis (EDA)

#### Univariate Analysis

- **Numerical Columns**: Distribution analysis using histograms and boxplots
  - `total_bill` distribution
  - `tip` distribution
  - `size` distribution
- **Categorical Columns**: Frequency analysis using count plots
  - `day` distribution
  - `time` distribution
  - `sex` distribution
  - `smoker` distribution

#### Bivariate Analysis

- Correlation heatmap for numerical columns
- Scatter plots to understand relationships between `total_bill` and `tip`
- Strip plots and box plots for categorical vs numerical analysis

#### Multivariate Analysis

- Relationship between `total_bill` and `tip` segmented by:
  - Gender of bill payer
  - Smoking status
  - Day of visit
  - Time of visit (Lunch/Dinner)
  - Group size

### 3. Key Questions Answered

- How do bill amounts and tips vary by day of the week?
- Which time of day brings in higher bill and tip amounts?
- Does the gender of the bill payer affect tipping behavior?
- Is there a relationship between smoking status and tips?
- How does group size affect the relationship between bill and tip?

---

## 💡 Key Insights & Findings

### Bill & Tip Distribution

- 📊 The bill amount ranges from ~$3 to ~$51 with an average of ~$20
- 💵 The tip amount ranges from ~$1 to ~$10 with mean and median both ~$3
- 👥 Group size varies from 1 to 6 people
- 📈 50% of customers pay less than $20 for their overall bill

### Bill-Tip Relationship

- 📈 **Strong linear relationship** between `total_bill` and `tip` - higher bills lead to higher tips
- 🚬 Non-smokers show a more prominent linear relationship than smokers
- 👨‍👩‍👧‍👦 This relationship becomes more constant as group size increases

### Day & Time Patterns

- 📅 **Weekends (Sat/Sun)** have higher order counts compared to weekdays
- 🍽️ **Dinner time** has significantly more orders than lunch
- 💰 Median billing amount is higher on Saturdays and Sundays
- 🕐 Customers spend ~$19 during dinner vs ~$16 during lunch (median)
- 💵 Dinner tips are ~$1 higher than lunch tips on average

### Gender Patterns

- 👔 Male bill payers (~160) are almost **double** the number of female payers (~80)
- 📆 On weekends, male bill payers significantly outnumber females
- ⚖️ Median tip amount is roughly equal for both genders
- 📊 Males have more outliers giving higher tips

### Smoker Patterns

- 🚭 Non-smokers outnumber smokers by approximately 60
- 📆 Non-smokers are significantly more common on Thursdays and Sundays
- 🗓️ Only on Fridays do smokers outnumber non-smokers
- ⚖️ **No significant relationship** between smoking status and tip amount

---

## 📈 Visualizations

The analysis includes various visualization types:

| Visualization Type      | Purpose                                           |
| ----------------------- | ------------------------------------------------- |
| **Histogram**           | Distribution of numerical variables               |
| **Boxplot**             | Outlier detection and quartile analysis           |
| **Countplot**           | Frequency distribution of categorical variables   |
| **Correlation Heatmap** | Relationship strength between numerical variables |
| **Scatter Plot**        | Relationship between total_bill and tip           |
| **Strip Plot**          | Distribution with jitter for overlapping points   |
| **Regression Plot**     | Linear relationship with confidence intervals     |

---

## 🚀 How to Run

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Steps to Execute

1. Clone or download the repository
2. Navigate to the `tips/` directory
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Tips_Case_Study.ipynb
   ```
4. Run all cells sequentially to reproduce the analysis

### Quick Start with Python

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the data
tips = pd.read_csv('tips.csv')

# Quick overview
print(tips.head())
print(tips.describe())

# Quick visualization
sns.scatterplot(data=tips, x='total_bill', y='tip', hue='day')
plt.show()
```

---

## 📚 Learning Outcomes

By completing this case study, you will learn:

1. **Data Loading & Cleaning**: How to load CSV data and preprocess it for analysis
2. **Exploratory Data Analysis**: Techniques to understand data distributions and patterns
3. **Data Visualization**: Creating meaningful plots using Matplotlib and Seaborn
4. **Statistical Analysis**: Understanding correlation and relationships between variables
5. **Business Insights**: Translating data patterns into actionable business recommendations

---

## 📝 Author

This case study is part of the Python Foundations learning track, designed to provide hands-on experience with real-world data analysis scenarios.

---

## 📜 License

This project is for educational purposes.
