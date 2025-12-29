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
    └── food-hub/
        ├── README.md                  # FoodHub case study documentation
        ├── foodhub.ipynb              # Jupyter notebook with analysis
        └── foodhub_order.csv          # Dataset
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
