# 🚗 Austo Automobile Case Study

## Python Foundations Project | Customer Profile Analysis for US Market Entry

---

## 📋 Table of Contents

- [Background](#-background)
- [Business Objective](#-business-objective)
- [Dataset Description](#-dataset-description)
- [Data Dictionary](#-data-dictionary)
- [Analysis Framework](#-analysis-framework)
- [Key Questions to Explore](#-key-questions-to-explore)
- [Technologies Used](#-technologies-used)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [Expected Outcomes](#-expected-outcomes)

---

## 🌍 Background

In the 21st century, cars are an essential mode of transportation that provides personal control and autonomy. In day-to-day life, people use cars for commuting to work, shopping, visiting family and friends, and more. Research shows that **more than 76% of people** limit their travel destinations when they don't have access to a car.

**Austo**, a UK-based automobile company, has successfully established its footprints in the European market and now aspires to **expand into the US market**. To understand the types of cars preferred by American customers and the factors influencing car purchase behavior, Austo has contracted a consulting firm.

Based on various market surveys, the consulting firm has created a comprehensive dataset covering **3 major types of cars** that are extensively used across the US market, along with detailed information about car owners.

---

## 🎯 Business Objective

Austo's management team wants to achieve the following:

1. **Understand buyer demand** and trends in the US market
2. **Build customer profiles** based on data analysis to identify new purchase opportunities
3. **Manipulate business strategy** and production to meet specific demand levels
4. **Comprehend market dynamics** of the new US market

As a Data Scientist at the consulting firm, the task is to:

- Create **buyer profiles** for different types of cars
- Provide **data-driven recommendations** for Austo
- Generate **actionable insights** to help Austo grow its business in the US

---

## 📊 Dataset Description

| File                   | Description                                                          |
| ---------------------- | -------------------------------------------------------------------- |
| `austo_automobile.csv` | Contains buyer data corresponding to different types of car products |

The dataset captures comprehensive information about car buyers including demographics, financial status, loan history, and the type of car purchased.

---

## 📖 Data Dictionary

| Column             | Description                                                   | Type        |
| ------------------ | ------------------------------------------------------------- | ----------- |
| `Age`              | Age of the customer                                           | Numerical   |
| `Gender`           | Gender of the customer                                        | Categorical |
| `Profession`       | Whether the customer is a Salaried or Business person         | Categorical |
| `Marital_status`   | Marital status of the customer (Single/Married)               | Categorical |
| `Education`        | Highest level of education completed (Graduate/Post Graduate) | Categorical |
| `No_of_Dependents` | Number of dependents (partner/children/spouse)                | Numerical   |
| `Personal_loan`    | Whether the customer availed a personal loan (Yes/No)         | Categorical |
| `House_loan`       | Whether the customer availed a house loan (Yes/No)            | Categorical |
| `Partner_working`  | Whether the customer's partner is working (Yes/No)            | Categorical |
| `Salary`           | Annual salary of the customer (in USD)                        | Numerical   |
| `Partner_salary`   | Annual salary of the customer's partner (in USD)              | Numerical   |
| `Total_salary`     | Annual household income (Salary + Partner_salary)             | Numerical   |
| `Price`            | Price of the car purchased (in USD)                           | Numerical   |
| `Make`             | Car type - Hatchback, Sedan, or SUV                           | Categorical |

---

## 🔬 Analysis Framework

The analysis is structured into the following phases:

### 1. Data Overview

- Understanding data dimensions (rows and columns)
- Examining data types
- Statistical summary analysis
- Missing value detection and treatment

### 2. Univariate Analysis

- Distribution analysis for numerical variables (Age, Salary, Price, etc.)
- Frequency analysis for categorical variables (Gender, Profession, Make, etc.)
- Using histograms, boxplots, and countplots for visualization

### 3. Multivariate Analysis

- Exploring relationships between numerical variables
- Analyzing relationships between numerical and categorical variables
- Understanding how demographics influence car purchase decisions

### 4. Insights & Recommendations

- Drawing business conclusions
- Building customer profiles
- Providing strategic recommendations for US market entry

---

## ❓ Key Questions to Explore

The case study addresses the following analytical questions:

| #   | Question                                                                                   | Marks |
| --- | ------------------------------------------------------------------------------------------ | ----- |
| 1   | How many rows and columns are present in the data?                                         | 0.5   |
| 2   | What are the datatypes of different columns?                                               | 0.5   |
| 3   | What is the minimum, average, and maximum Price of cars?                                   | 2     |
| 4   | Are there any missing values? How to treat them?                                           | 1     |
| 5   | How many cars are of type SUV?                                                             | 1     |
| 6   | Explore all variables and provide distribution observations                                | 10    |
| 7   | How many Hatchback cars are priced above $25,000?                                          | 2     |
| 8   | How many owners bought cars priced higher than their salary? How many took personal loans? | 3     |
| 9   | Perform multivariate analysis to explore relationships                                     | 15    |
| 10  | For customers with ≤3 dependents, how does average car price vary by profession?           | 2     |
| 11  | For customers with both home loan and personal loan, how does price vary by profession?    | 3     |
| 12  | Write conclusions and business recommendations                                             | 6     |

**Total Marks: 46**

---

## 🛠️ Technologies Used

| Technology                                                                                          | Version | Purpose                   |
| --------------------------------------------------------------------------------------------------- | ------- | ------------------------- |
| ![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python&logoColor=white)                | 3.9+    | Programming Language      |
| ![NumPy](https://img.shields.io/badge/NumPy-1.25.2-013243?logo=numpy&logoColor=white)               | 1.25.2  | Numerical Computing       |
| ![Pandas](https://img.shields.io/badge/Pandas-1.5.3-150458?logo=pandas&logoColor=white)             | 1.5.3   | Data Manipulation         |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7.1-11557c?logo=matplotlib&logoColor=white) | 3.7.1   | Data Visualization        |
| ![Seaborn](https://img.shields.io/badge/Seaborn-0.13.1-9cf?logo=seaborn&logoColor=white)            | 0.13.1  | Statistical Visualization |

---

## 🚀 Getting Started

### Prerequisites

Ensure you have Python 3.9+ installed on your system.

### Installation

1. **Clone the repository** (if applicable):

   ```bash
   git clone <repository-url>
   cd case-studies/austo
   ```

2. **Install required libraries**:

   ```bash
   pip install numpy==1.25.2 pandas==1.5.3 matplotlib==3.7.1 seaborn==0.13.1
   ```

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook austo_project.ipynb
   ```

### Running on Google Colab

1. Upload the notebook to Google Colab
2. Upload `austo_automobile.csv` to your Google Drive
3. Uncomment and run the drive mount cells in the notebook
4. Update the file path to match your Drive location

---

## 📁 Project Structure

```
austo/
├── README.md                  # Project documentation (this file)
├── austo_automobile.csv       # Dataset with customer and car purchase data
└── austo_project.ipynb        # Jupyter notebook with analysis questions
```

---

## 🎯 Expected Outcomes

Upon completing this case study, you will be able to:

### Customer Profiles

- **Hatchback Buyers**: Typically younger customers, potentially with more dependents, lower-middle income bracket
- **Sedan Buyers**: Middle-aged customers, moderate income, possibly with working partners
- **SUV Buyers**: Older customers with higher income levels, potentially fewer dependents

### Business Insights

- Understanding of key demographic factors influencing car type preference
- Insights into the relationship between income levels and car pricing
- Analysis of loan behavior patterns among car buyers
- Identification of potential target segments for each car type

### Strategic Recommendations

Based on the analysis, provide actionable recommendations for:

- Target market segments for each car type
- Pricing strategies for the US market
- Marketing approaches for different customer profiles
- Product mix optimization for US market entry

---

## 📝 Notes

- **Restart the kernel** after installing libraries when running on Colab
- All observations should be documented in the designated markdown cells
- Focus on deriving actionable business insights, not just statistical findings
- Consider both individual variable distributions and inter-variable relationships

---

## 🤝 Contributing

This is an educational case study project. Feel free to:

- Fork the repository and add your own analysis
- Share insights and findings
- Suggest improvements to the analysis approach

---

## 📄 License

This project is part of the Python Foundations curriculum and is intended for educational purposes.

---

<div align="center">

**Happy Analyzing! 📊🚗**

_Helping Austo understand the US automobile market through data-driven insights_

</div>
