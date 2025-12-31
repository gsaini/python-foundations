# 🐍 Python Foundations

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)

The objective is to get a holistic overview of solving a business problem through analytics and to set up the foundations of the skills required to work with data, delivered via the foundations of Python.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Case Studies](#case-studies)
- [Skills Covered](#skills-covered)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Reference Material](#reference-material)

---

## 🎯 Overview

This repository contains hands-on case studies and projects designed to build a strong foundation in Python for data analysis. Each case study focuses on real-world business scenarios, helping you develop practical skills in:

- Data manipulation and cleaning
- Exploratory Data Analysis (EDA)
- Statistical analysis
- Data visualization
- Deriving actionable business insights

---

## 📚 Case Studies

### 1. 🍽️ Tips Case Study

**Location:** [`case-studies/tips/`](./case-studies/tips/)

Analyze tipping patterns at Chef's Kitchen restaurant in San Diego to understand customer behavior and identify trends in revenue and tips across different demographics.

| Aspect              | Details                                                      |
| ------------------- | ------------------------------------------------------------ |
| **Business Domain** | Restaurant / Hospitality                                     |
| **Dataset Size**    | 244 records, 8 features                                      |
| **Key Variables**   | total_bill, tip, day, time, size, smoker, sex                |
| **Analysis Focus**  | Tipping behavior, customer demographics, time-based patterns |

**Key Questions Answered:**

- What is the relationship between bill amount and tip?
- How do tips vary by day of the week and time of day?
- Does gender or smoking status affect tipping behavior?
- How does group size impact tipping patterns?

📖 [View Full Documentation](./case-studies/tips/README.md)

---

### 2. 🍔 FoodHub Case Study

**Location:** [`case-studies/food-hub/`](./case-studies/food-hub/)

Analyze order data from FoodHub, a food aggregator company in New York, to understand restaurant demand and enhance customer experience.

| Aspect              | Details                                                              |
| ------------------- | -------------------------------------------------------------------- |
| **Business Domain** | Food Delivery / E-commerce                                           |
| **Dataset Size**    | Large-scale order data                                               |
| **Key Variables**   | order_id, restaurant_name, cuisine_type, cost, rating, delivery_time |
| **Analysis Focus**  | Restaurant performance, delivery efficiency, customer satisfaction   |

**Key Questions Answered:**

- Which restaurants and cuisine types are most popular?
- How do order costs vary across different restaurants?
- What factors affect delivery time and customer ratings?
- Are there patterns in weekday vs weekend orders?

📖 [View Full Documentation](./case-studies/food-hub/README.md)

---

### 3. 🍯 Honey Production Case Study

**Location:** [`case-studies/honey-production/`](./case-studies/honey-production/)

Explore the decline of honey production in the United States from 1998 to 2016, investigating the impact of Colony Collapse Disorder (CCD) and analyzing trends in production, pricing, and state-level performance.

| Aspect              | Details                                                                    |
| ------------------- | -------------------------------------------------------------------------- |
| **Business Domain** | Agriculture / Environmental Science                                        |
| **Dataset Size**    | 786 records, 8 features (19 years: 1998-2016)                              |
| **Key Variables**   | state, numcol, yieldpercol, totalprod, stocks, priceperlb, prodvalue, year |
| **Analysis Focus**  | Production trends, colony decline, pricing dynamics, state-level patterns  |

**Key Questions Answered:**

- How has honey production yield changed from 1998 to 2016?
- What are the major production trends across states over time?
- Are there patterns between total honey production and value of production each year?
- Which states are the largest honey producers and which produce the most expensive honey?

**Key Findings:**

- 📉 Overall honey production in the US has been decreasing over the years
- 🐝 Decline attributed to both decreasing colonies AND decreasing yield per colony
- 🏆 Top producers: North Dakota, California, South Dakota, Florida, Montana
- 💰 Virginia produces the costliest honey; Oklahoma produces the cheapest

📖 [View Full Documentation](./case-studies/honey-production/README.md)

---

### 4. 📱 Google Play Store Case Study (Zoom Ads)

**Location:** [`case-studies/google-play-store/`](./case-studies/google-play-store/)

Analyze Google Play Store data for Zoom Ads, an advertising agency looking to identify trending Android applications for targeted advertisement promotion to maximize profit.

| Aspect              | Details                                                                             |
| ------------------- | ----------------------------------------------------------------------------------- |
| **Business Domain** | Digital Advertising / Mobile App Market                                             |
| **Dataset Size**    | App store data with 12 features                                                     |
| **Key Variables**   | App, Category, Rating, Reviews, Size, Installs, Price, Content Rating, Ad Supported |
| **Analysis Focus**  | App trends, market analysis, advertising opportunities, user engagement patterns    |

**Context:**

Android is the mobile operating system running on Google OS with about **69% of the market share worldwide**. The Google Play Store is the Android app store used to install Android Apps. Zoom Ads wants to understand app trends to focus advertising efforts on applications that are trending and can lead to maximum profit.

**Key Questions Answered:**

- Which app categories are most popular on the Google Play Store?
- What is the relationship between app ratings and number of installs?
- How do free vs paid apps compare in terms of user engagement?
- Which apps support advertisements and have high user engagement?
- What content ratings attract the most users?

**Analysis Guidelines:**

- 📊 Univariate analysis to understand individual variable distributions
- 🔗 Bivariate analysis to explore correlations between variables
- 📈 Visualizations to extract actionable insights for advertising strategy

**Data Features:**

| Feature            | Description                                            |
| ------------------ | ------------------------------------------------------ |
| `App`              | Application Name                                       |
| `Category`         | Category the app belongs to                            |
| `Rating`           | Overall user rating of the app                         |
| `Reviews`          | Number of user reviews for the app                     |
| `Size`             | Size of the app in kilobytes                           |
| `Installs`         | Number of user downloads/installs for the app          |
| `Price`            | Price of an app in dollars                             |
| `Paid/Free`        | Whether an app is paid or free (Yes/No)                |
| `Content Rating`   | Age group the app is targeted at                       |
| `Ad Supported`     | Whether an app supports an Ad or not (Yes/No)          |
| `In App Purchases` | App containing in-app purchase feature or not (Yes/No) |
| `Editors Choice`   | Whether rated as Editor's Choice (Yes/No)              |

📖 [View Full Documentation](./case-studies/google-play-store/README.md)

---

## 🛠️ Skills Covered

| Skill Category           | Topics                                                              |
| ------------------------ | ------------------------------------------------------------------- |
| **Python Basics**        | Data types, loops, conditionals, functions, list comprehensions     |
| **Data Manipulation**    | Pandas DataFrames, data cleaning, filtering, grouping, aggregation  |
| **Data Visualization**   | Matplotlib, Seaborn (histograms, boxplots, scatter plots, heatmaps) |
| **Statistical Analysis** | Descriptive statistics, correlation, distribution analysis          |
| **Business Analytics**   | Deriving insights, identifying patterns, making recommendations     |

---

## 💻 Technologies Used

| Technology           | Purpose                             |
| -------------------- | ----------------------------------- |
| **Python 3.x**       | Core programming language           |
| **Pandas**           | Data manipulation and analysis      |
| **NumPy**            | Numerical computations              |
| **Matplotlib**       | Basic plotting and visualization    |
| **Seaborn**          | Statistical data visualization      |
| **Jupyter Notebook** | Interactive development environment |

---

## 📁 Project Structure

```
python-foundations/
├── README.md                          # This file
└── case-studies/
    ├── tips/
    │   ├── README.md                  # Tips case study documentation
    │   ├── Tips_Case_Study.ipynb      # Jupyter notebook with analysis
    │   └── tips.csv                   # Dataset
    ├── food-hub/
    │   ├── README.md                  # FoodHub case study documentation
    │   ├── foodhub.ipynb              # Jupyter notebook with analysis
    │   └── foodhub_order.csv          # Dataset
    ├── honey-production/
    │   ├── README.md                  # Honey production case study documentation
    │   ├── Session_Notebook_Honey_Production_Case_Study.ipynb  # Jupyter notebook
    │   └── honeyproduction1998-2016.csv  # Dataset (1998-2016)
    └── google-play-store/
        ├── README.md                  # Google Play Store case study documentation
        ├── Google_Play_Store_Case_Study.ipynb  # Jupyter notebook with analysis
        └── google_play_store.csv      # Google Play Store dataset
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.x installed along with the following libraries:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Case Studies

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd python-foundations
   ```

2. **Launch Jupyter Notebook:**

   ```bash
   jupyter notebook
   ```

3. **Navigate to a case study and open the `.ipynb` file**

4. **Run all cells** to reproduce the analysis

---

## 📖 Reference Material

Here is a curated list of resources to deepen your Python data analysis skills:

### Data Visualization

- [Data Visualization — How to Pick the Right Chart Type?](https://medium.com/@mokkup/data-visualization-how-to-pick-the-right-chart-type-f6f65824928a)
- [Explore more with the functionalities of the Seaborn library](http://seaborn.pydata.org/examples/index.html)

### Exploratory Data Analysis

- [An Extensive Step by Step Guide to Exploratory Data Analysis](https://ankushmulkar.medium.com/complete-exploratory-data-analysis-step-by-step-guide-for-data-analyst-34a07156217a)

### Data Cleaning & Preprocessing

- [When Should You Delete Outliers from a Data Set?](https://humansofdata.atlan.com/2018/03/when-delete-outliers-dataset/)
- [How to Handle Missing Data with Python](https://machinelearningmastery.com/handle-missing-data-python/)
- [Selecting the appropriate outlier treatment](https://www.lexjansen.com/nesug/nesug07/sa/sa16.pdf)
- [Why 1.5 Is Used in the IQR Rule for Outlier Detection](https://builtin.com/articles/1-5-iqr-rule)

### Python Programming

- [List Comprehension, Conditional, and Looping Statements](https://medium.com/geekculture/list-comprehension-conditional-and-looping-statements-in-python-16db4ea9e58b)
- [All About Python List Comprehension](https://towardsdatascience.com/all-about-python-list-comprehension-14dd979ec0d1/)

### Libraries & Tools

- [Why Should We Use NumPy?](https://medium.com/fintechexplained/why-should-we-use-numpy-c14a4fb03ee9)
- [The pandas DataFrame: Make Working With Data Delightful](https://realpython.com/pandas-dataframe/)
- [Guidelines for working with external data in Google Colab](https://colab.research.google.com/notebooks/io.ipynb)

### Text Processing

- [How to Clean Text for Machine Learning with Python](https://machinelearningmastery.com/clean-text-machine-learning-python/)

---

## 📝 License

This project is for educational purposes.

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

- Add new case studies
- Improve existing documentation
- Fix bugs or enhance code quality
- Add additional reference materials
