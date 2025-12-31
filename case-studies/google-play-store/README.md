# 📱 Google Play Store Case Study (Zoom Ads)

A comprehensive data analysis project exploring the Android app market on Google Play Store to identify trending applications for targeted advertisement promotion and maximize advertising profit for Zoom Ads.

---

## 📋 Table of Contents

- [Background](#background)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Key Analysis Steps](#key-analysis-steps)
- [Key Questions to Answer](#key-questions-to-answer)
- [Expected Insights](#expected-insights)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)

---

## 🎯 Background

### The Digital Advertising Landscape

**Advertising** is a type of marketing communication used to promote or sell products or services. Advertising is usually paid by sponsors and viewed through various media such as:

- 🌐 Websites
- 📱 Mobile Apps
- 📧 Emails
- 📺 Other offline communications

### Android Market Dominance

- **Android** is the mobile operating system running on Google OS
- Commands approximately **69% of the market share worldwide**
- The **Google Play Store** is the official Android app store used to install Android applications
- Millions of apps available across various categories

### Business Context

**Zoom Ads** is an advertising agency looking to capitalize on the mobile app market. Understanding app trends, user engagement patterns, and advertisement support across applications is crucial for making data-driven decisions on where to focus advertising efforts.

---

## 🎯 Objective

As a **Data Scientist** at Zoom Ads, the goal is to:

1. **Gather and analyze** detailed information on apps in the Google Play Store
2. **Identify trending applications** that can be targeted for advertisement promotion
3. **Provide actionable insights** on app features and the current state of the Android app market
4. **Maximize advertising profit** by focusing on high-engagement applications

### Analysis Guidelines

| Analysis Type           | Purpose                                               |
| ----------------------- | ----------------------------------------------------- |
| **Univariate Analysis** | Understand individual variable distributions          |
| **Bivariate Analysis**  | Explore correlations between different variables      |
| **Visualizations**      | Extract insights and communicate findings effectively |

---

## 📊 Dataset Description

The dataset contains information about applications on the Google Play Store with the following **12 features**:

| Feature            | Description                                            | Data Type   |
| ------------------ | ------------------------------------------------------ | ----------- |
| `App`              | Application Name                                       | Categorical |
| `Category`         | Category the app belongs to                            | Categorical |
| `Rating`           | Overall user rating of the app (1-5 scale)             | Float       |
| `Reviews`          | Number of user reviews for the app                     | Integer     |
| `Size`             | Size of the app in kilobytes                           | Float       |
| `Installs`         | Number of user downloads/installs for the app          | Integer     |
| `Price`            | Price of an app in dollars                             | Float       |
| `Paid/Free`        | Whether an app is paid or free (Yes/No)                | Categorical |
| `Content Rating`   | Age group the app is targeted at                       | Categorical |
| `Ad Supported`     | Whether an app supports an Ad or not (Yes/No)          | Categorical |
| `In App Purchases` | App containing in-app purchase feature or not (Yes/No) | Categorical |
| `Editors Choice`   | Whether rated as Editor's Choice (Yes/No)              | Categorical |

### Key Feature Categories

#### Engagement Metrics

- **Rating**: Indicates user satisfaction
- **Reviews**: Reflects user engagement level
- **Installs**: Shows app popularity and reach

#### Monetization Features

- **Price**: Direct revenue from paid apps
- **Ad Supported**: Potential for ad revenue
- **In App Purchases**: Alternative monetization strategy

#### App Characteristics

- **Category**: Market segment classification
- **Content Rating**: Target audience demographics
- **Editors Choice**: Quality indicator from Google

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
google-play-store/
├── README.md                                    # Project documentation (this file)
├── Google_Play_Store_Case_Study.ipynb           # Jupyter notebook with complete analysis
└── google_play_store.csv                        # Dataset file
```

---

## 🔍 Key Analysis Steps

### 1. Data Loading & Preprocessing

- Import necessary libraries (pandas, numpy, matplotlib, seaborn)
- Load the dataset from CSV
- Handle missing values and data inconsistencies
- Convert data types as needed (e.g., Installs, Size, Price)
- Get statistical summary of the data

### 2. Univariate Analysis

Analysis of individual variables to understand distributions:

#### Numerical Variables

- **Rating** distribution - How are apps rated overall?
- **Reviews** distribution - What's the typical engagement level?
- **Size** distribution - How large are most apps?
- **Installs** distribution - What's the typical download range?
- **Price** distribution - How are paid apps priced?

#### Categorical Variables

- **Category** distribution - Which categories have the most apps?
- **Content Rating** distribution - What age groups are targeted?
- **Paid/Free** distribution - Ratio of free vs paid apps
- **Ad Supported** distribution - How many apps support ads?
- **In App Purchases** distribution - IAP adoption rate
- **Editors Choice** distribution - Quality app percentage

### 3. Bivariate Analysis

Exploring relationships between variables:

- **Rating vs Installs**: Do higher-rated apps get more downloads?
- **Category vs Rating**: Which categories have the best ratings?
- **Free vs Paid**: How do engagement metrics differ?
- **Ad Supported vs Installs**: Do ad-supported apps have higher reach?
- **Size vs Rating**: Does app size affect user satisfaction?
- **Reviews vs Rating**: Correlation between engagement and satisfaction

### 4. Advertising Opportunity Analysis

- Identify high-engagement apps that support advertisements
- Analyze categories with the best advertising potential
- Compare free vs paid apps for ad opportunities
- Evaluate content ratings for target audience reach

---

## ❓ Key Questions to Answer

### Market Overview

1. **What is the distribution of apps across different categories?**
2. **What is the ratio of free vs paid applications?**
3. **How are apps distributed across different content ratings?**

### User Engagement

4. **Which app categories have the highest user ratings?**
5. **Is there a correlation between the number of reviews and app rating?**
6. **What is the relationship between app installs and ratings?**

### Advertising Insights

7. **What percentage of apps support advertisements?**
8. **Which categories have the highest proportion of ad-supported apps?**
9. **Do ad-supported apps have higher or lower ratings compared to non-ad apps?**
10. **Which ad-supported apps have the highest number of installs?**

### Monetization Analysis

11. **How do in-app purchase apps compare to non-IAP apps in terms of engagement?**
12. **What is the price distribution of paid apps?**
13. **Are Editor's Choice apps more likely to support advertisements?**

---

## 💡 Expected Insights

### Market Trends

- 📊 Category distribution and market saturation
- 📈 Growth potential in underserved categories
- 🎯 Target demographics based on content ratings

### Advertising Opportunities

- 💰 High-engagement apps with ad support
- 🏆 Top-performing categories for ad placement
- 📱 Free apps with maximum reach for ad revenue

### User Behavior Patterns

- ⭐ Factors influencing app ratings
- 📥 Download patterns across categories
- 💬 Review engagement indicators

### Strategic Recommendations

- 🎯 Focus areas for Zoom Ads campaigns
- 📊 Data-driven category prioritization
- 💵 ROI potential based on engagement metrics

---

## 📈 Visualizations

The analysis should include various visualization types:

| Visualization Type | Purpose                                          |
| ------------------ | ------------------------------------------------ |
| **Bar Charts**     | Category distribution, content rating comparison |
| **Histograms**     | Distribution of ratings, reviews, installs       |
| **Box Plots**      | Rating/reviews comparison across categories      |
| **Pie Charts**     | Free vs paid ratio, ad-supported ratio           |
| **Scatter Plots**  | Correlation between numerical variables          |
| **Heatmaps**       | Correlation matrix of numerical features         |
| **Count Plots**    | Categorical variable frequencies                 |
| **Violin Plots**   | Distribution comparison across groups            |

---

## 🚀 How to Run

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Steps to Execute

1. Clone or download the repository
2. Navigate to the `google-play-store/` directory
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Google_Play_Store_Case_Study.ipynb
   ```
4. Run all cells sequentially to reproduce the analysis

### Quick Start with Python

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the data
playstore = pd.read_csv('google_play_store.csv')

# Quick overview
print(playstore.head())
print(playstore.info())
print(playstore.describe())

# View category distribution
plt.figure(figsize=(14, 8))
sns.countplot(y='Category', data=playstore, order=playstore['Category'].value_counts().index)
plt.title('App Distribution by Category')
plt.xlabel('Number of Apps')
plt.ylabel('Category')
plt.tight_layout()
plt.show()

# Analyze ad-supported apps
ad_supported = playstore['Ad Supported'].value_counts()
print(f"\nAd Supported Apps: {ad_supported}")
```

---

## 📚 Learning Outcomes

By completing this case study, you will learn:

1. **Market Analysis**: Understanding app market dynamics and trends
2. **Univariate Analysis**: Exploring individual variable distributions
3. **Bivariate Analysis**: Discovering relationships between features
4. **Data Visualization**: Creating meaningful charts for business insights
5. **Business Analytics**: Translating data findings into advertising strategy

---

## 🌍 Real-World Relevance

This case study is particularly valuable because:

- **Digital Marketing**: Understanding where to place advertisements for maximum ROI
- **Market Research**: Analyzing competitive landscape in the app market
- **Business Strategy**: Data-driven decision making for advertising investments
- **Trend Analysis**: Identifying emerging categories and opportunities

---

## 📝 Conclusion

This analysis aims to provide Zoom Ads with:

1. **Market Understanding**: Comprehensive view of the Google Play Store ecosystem
2. **Target Identification**: High-potential apps and categories for ad placement
3. **Engagement Insights**: Understanding user behavior patterns
4. **Strategic Direction**: Data-backed recommendations for advertising campaigns
5. **ROI Optimization**: Focus on apps with maximum advertising potential

These findings will enable Zoom Ads to make informed decisions about where to invest advertising resources for maximum profit.

---

## 📜 License

This project is for educational purposes.
