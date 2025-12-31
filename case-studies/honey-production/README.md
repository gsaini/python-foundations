# 🍯 Honey Production Case Study

A comprehensive data analysis project exploring the decline of honey production in the United States from 1998 to 2016. This case study investigates the impact of Colony Collapse Disorder and analyzes trends in honey production, pricing, and state-level performance.

---

## 📋 Table of Contents

- [Background](#background)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Key Analysis Steps](#key-analysis-steps)
- [Key Questions Answered](#key-questions-answered)
- [Key Insights & Findings](#key-insights--findings)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)

---

## 🎯 Background

In **2006**, global concern was raised over the rapid decline in the honeybee population, an integral component of American honey agriculture. Large numbers of hives were lost to **Colony Collapse Disorder (CCD)**, a phenomenon where worker bees mysteriously disappear, causing the remaining hive colony to collapse.

### The Colony Collapse Crisis

- **Speculation on causes**: Hive diseases and pesticides harming pollinators (no overall consensus reached)
- **Impact on U.S. honey production**: The U.S. used to locally produce over half the honey it consumes per year
- **Current state**: Now, honey mostly comes from overseas, with **350 of 400 million pounds** consumed every year originating from imports

This dataset provides critical insights into honey production supply and demand in America during this transformative period (1998-2016).

---

## 🎯 Objective

To **visualize and analyze how honey production has changed over the years (1998-2016)** in the United States, including:

1. Understanding long-term production trends
2. Identifying state-level production patterns
3. Analyzing the relationship between production volume and market value
4. Examining the economic impact of declining production

---

## 📊 Dataset Description

The dataset contains **786 records** spanning **19 years** (1998-2016) with the following **8 features**:

| Feature       | Description                                                                                      | Data Type   |
| ------------- | ------------------------------------------------------------------------------------------------ | ----------- |
| `state`       | U.S. state where honey was produced                                                              | Categorical |
| `numcol`      | Number of honey-producing colonies (maximum colonies from which honey was taken during the year) | Integer     |
| `yieldpercol` | Honey yield per colony (pounds)                                                                  | Float       |
| `totalprod`   | Total production (numcol × yieldpercol) in pounds                                                | Integer     |
| `stocks`      | Stocks held by producers (pounds)                                                                | Integer     |
| `priceperlb`  | Average price per pound based on expanded sales (dollars)                                        | Float       |
| `prodvalue`   | Value of production (totalprod × priceperlb) in dollars                                          | Integer     |
| `year`        | Year of production (1998-2016)                                                                   | Integer     |

### Important Notes:

- Certain states are excluded every year (e.g., CT) to avoid disclosing data for individual operations
- Due to rounding, total colonies multiplied by total yield may not exactly equal production
- Summation of state values may not equal U.S. level value of production

### Data Source

[Kaggle - Honey Production Dataset](https://www.kaggle.com/jessicali9530/honey-production)

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
honey-production/
├── README.md                                           # Project documentation (this file)
├── Session_Notebook_Honey_Production_Case_Study.ipynb  # Jupyter notebook with complete analysis
└── honeyproduction1998-2016.csv                        # Dataset file
```

---

## 🔍 Key Analysis Steps

### 1. Data Loading & Preprocessing

- Import necessary libraries (pandas, numpy, matplotlib, seaborn)
- Load the dataset from CSV
- Verify data types and check for missing values
- Get statistical summary of the data

### 2. Univariate Analysis

Analysis of individual numerical variables using histograms and distribution plots:

- **Number of honey-producing colonies** distribution
- **Yield per colony** distribution
- **Total honey production** distribution
- **Price per pound** distribution
- **Value of production** distribution
- **Stocks held by producers** distribution

### 3. Correlation Analysis

- Correlation heatmap to understand relationships between numerical variables
- Identify strong correlations between production metrics

### 4. State-Level Analysis

- States with **maximum and minimum** honey production
- States producing the **costliest and cheapest** honey
- Average price per pound across all states

### 5. Time Series Analysis

Trend analysis over the years (1998-2016):

- **Overall trend of honey production in the US**
- **Variation in the number of colonies** over years
- **Variation of yield per colony** over years
- Production trends at **state level**
- Yearly trend in colonies and yield for the **5 prominent states**

### 6. Economic Analysis

- Effect of declining production on the **value of production**
- Comparison of **total production vs stocks** held by producers per state

---

## ❓ Key Questions Answered

1. **How has honey production yield changed from 1998 to 2016?**
2. **What are the major production trends across the states over time?**
3. **Are there patterns between total honey production and value of production each year?**
4. **How has the value of production (tied to demand) changed every year?**
5. **Which states are the largest honey producers?**
6. **Which states produce the most expensive honey?**

---

## 💡 Key Insights & Findings

### Production Trends

- 📉 **Overall honey production in the US has been decreasing** over the years (1998-2016)
- 📊 Total honey production = Number of colonies × Average yield per colony
- 🐝 The decline is attributed to **both factors**: decreasing colonies AND decreasing yield per colony

### State-Level Insights

- 🏆 **Top honey-producing states**: North Dakota, California, South Dakota, Florida, Montana
- 💰 **Virginia** produces the costliest honey, followed by Illinois and North Carolina
- 💵 **Oklahoma** produces the cheapest honey on average, followed by Maryland and South Carolina

### Economic Observations

- 💹 Despite declining production, the **value of production** has shown interesting patterns
- 📈 Some states have been capitalizing on the supply shortage
- 🏭 The relationship between production and stocks reveals strategic holding patterns

### Colony Analysis

- 🔬 The number of honey-producing colonies has significantly declined
- 📉 Yield per colony has also shown a downward trend
- 🗺️ Different states show varying resilience to Colony Collapse Disorder

---

## 📈 Visualizations

The analysis includes various visualization types:

| Visualization Type   | Purpose                                      |
| -------------------- | -------------------------------------------- |
| **Histograms**       | Distribution of numerical variables          |
| **Bar Charts**       | State-wise production and pricing comparison |
| **Point Plots**      | Time series trends across years              |
| **Heatmap**          | Correlation between numerical variables      |
| **Line Plots**       | Year-over-year trend analysis                |
| **Multi-line Plots** | Comparing trends across prominent states     |

---

## 🚀 How to Run

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Steps to Execute

1. Clone or download the repository
2. Navigate to the `honey-production/` directory
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Session_Notebook_Honey_Production_Case_Study.ipynb
   ```
4. Run all cells sequentially to reproduce the analysis

### Quick Start with Python

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the data
honeyprod = pd.read_csv('honeyproduction1998-2016.csv')

# Quick overview
print(honeyprod.head())
print(honeyprod.describe())

# View production trend over years
plt.figure(figsize=(12, 6))
sns.pointplot(x='year', y='totalprod', data=honeyprod, estimator=sum, errorbar=None)
plt.xticks(rotation=90)
plt.title('US Honey Production Trend (1998-2016)')
plt.show()
```

---

## 📚 Learning Outcomes

By completing this case study, you will learn:

1. **Time Series Analysis**: How to analyze trends over multiple years
2. **Geospatial Insights**: Understanding state-level variations in production
3. **Correlation Analysis**: Identifying relationships between production metrics
4. **Data Visualization**: Creating meaningful trend and comparison plots
5. **Business Analysis**: Understanding supply-demand dynamics and pricing

---

## 🌍 Real-World Relevance

This case study is particularly relevant because:

- **Environmental Impact**: Highlights the importance of bee populations for agriculture
- **Economic Analysis**: Shows how supply changes affect pricing
- **Policy Implications**: Data-driven insights for agricultural policy decisions
- **Sustainability**: Understanding factors affecting long-term food production

---

## 📝 Conclusion

The analysis reveals significant concerns about the U.S. honey production industry:

1. **Decreasing Production**: Consistent decline in total honey production over the 18-year period
2. **Colony Decline**: The number of honey-producing colonies has significantly decreased
3. **Yield Impact**: Even existing colonies are producing less honey per colony
4. **Economic Shifts**: While production declines, price and value dynamics are changing
5. **State Variations**: Different states show varying patterns of resilience and adaptation

These findings underscore the importance of addressing Colony Collapse Disorder and supporting sustainable beekeeping practices.

---

## 📜 License

This project is for educational purposes.
