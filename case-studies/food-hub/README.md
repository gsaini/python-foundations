# 🍔 FoodHub Data Analysis Case Study

A comprehensive data analysis project exploring order data from FoodHub, a food aggregator company in New York, to understand restaurant demand patterns and enhance customer experience through data-driven insights.

---

## 📋 Table of Contents

- [Background](#background)
- [Objective](#objective)
- [Dataset Description](#dataset-description)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Key Analysis Steps](#key-analysis-steps)
- [Key Questions to Answer](#key-questions-to-answer)
- [Key Insights & Findings](#key-insights--findings)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)

---

## 🎯 Background

### The Food Delivery Landscape in New York

The number of restaurants in New York is increasing day by day. With hectic lifestyles becoming the norm, many rely on convenient food options:

- 👨‍🎓 **Students** with busy academic schedules
- 💼 **Professionals** with demanding work hours
- 👨‍👩‍👧‍👦 **Families** seeking convenient meal solutions

**Online food delivery services** have become a great option, providing access to good food from favorite restaurants without the hassle of cooking or dining out.

### About FoodHub

**FoodHub** is a food aggregator company that offers access to **multiple restaurants through a single smartphone app**. The platform streamlines the entire food ordering and delivery process:

#### How FoodHub Works:

```
┌─────────────┐    ┌─────────────┐    ┌─────────────┐    ┌─────────────┐
│  Customer   │───▶│ Restaurant  │───▶│  Delivery   │───▶│  Customer   │
│ Places Order│    │  Confirms   │    │   Pick-up   │    │  Receives   │
└─────────────┘    └─────────────┘    └─────────────┘    └─────────────┘
```

1. **Order Placement**: Customer orders food through the FoodHub app
2. **Restaurant Confirmation**: Restaurant receives and confirms the order
3. **Delivery Assignment**: App assigns a delivery person to pick up the order
4. **Pick-up**: Delivery person uses the map to reach the restaurant and waits for the food
5. **Transit**: After pick-up confirmation, delivery person travels to customer location
6. **Delivery**: Food is delivered and drop-off is confirmed in the app
7. **Rating**: Customer rates the order through the app

### Business Model

FoodHub earns revenue by collecting a **fixed margin of the delivery order** from partnered restaurants. Understanding order patterns and customer preferences is crucial for:

- 📈 Increasing order volume
- ⭐ Improving customer satisfaction
- 🤝 Strengthening restaurant partnerships
- 💰 Maximizing revenue

---

## 🎯 Objective

As a **Data Scientist** at FoodHub, the primary goals are to:

1. **Analyze order data** to understand demand patterns across different restaurants
2. **Identify factors** affecting customer experience and satisfaction
3. **Provide actionable insights** to enhance business operations
4. **Answer key business questions** posed by the Data Science team

### Business Value

The analysis will help FoodHub:

| Goal                         | Impact                                            |
| ---------------------------- | ------------------------------------------------- |
| Understand restaurant demand | Better resource allocation and partnerships       |
| Analyze delivery efficiency  | Improved delivery times and customer satisfaction |
| Study customer preferences   | Enhanced personalization and recommendations      |
| Identify peak periods        | Optimized staffing and restaurant coordination    |

---

## 📊 Dataset Description

The dataset contains order information from FoodHub's online portal with the following **9 features**:

| Feature                 | Description                                           | Data Type   |
| ----------------------- | ----------------------------------------------------- | ----------- |
| `order_id`              | Unique ID of the order                                | Integer     |
| `customer_id`           | ID of the customer who ordered the food               | Integer     |
| `restaurant_name`       | Name of the restaurant                                | Categorical |
| `cuisine_type`          | Cuisine ordered by the customer                       | Categorical |
| `cost_of_the_order`     | Cost of the order (in dollars)                        | Float       |
| `day_of_the_week`       | Whether order is placed on Weekday or Weekend         | Categorical |
| `rating`                | Rating given by the customer out of 5                 | Float       |
| `food_preparation_time` | Time (in minutes) taken by restaurant to prepare food | Integer     |
| `delivery_time`         | Time (in minutes) taken to deliver the food package   | Integer     |

### Feature Details

#### Time Calculations

- **Food Preparation Time**: Calculated as the difference between:

  - Restaurant's order confirmation timestamp
  - Delivery person's pick-up confirmation timestamp

- **Delivery Time**: Calculated as the difference between:
  - Delivery person's pick-up confirmation timestamp
  - Delivery person's drop-off confirmation timestamp

#### Day Classification

| Category    | Days                |
| ----------- | ------------------- |
| **Weekday** | Monday to Friday    |
| **Weekend** | Saturday and Sunday |

### Key Metrics Categories

| Category                 | Features                             | Business Relevance                |
| ------------------------ | ------------------------------------ | --------------------------------- |
| **Order Identification** | order_id, customer_id                | Tracking and customer analysis    |
| **Restaurant Info**      | restaurant_name, cuisine_type        | Demand and preference analysis    |
| **Financial**            | cost_of_the_order                    | Revenue and pricing analysis      |
| **Temporal**             | day_of_the_week                      | Peak period identification        |
| **Quality**              | rating                               | Customer satisfaction measurement |
| **Efficiency**           | food_preparation_time, delivery_time | Operational performance           |

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
food-hub/
├── README.md                  # Project documentation (this file)
├── foodhub.ipynb              # Jupyter notebook with complete analysis
└── foodhub_order.csv          # Dataset file
```

---

## 🔍 Key Analysis Steps

### 1. Data Loading & Exploration

- Import necessary libraries (pandas, numpy, matplotlib, seaborn)
- Load the dataset from CSV
- Understand data structure and dimensions
- Check data types and missing values
- Generate statistical summary

### 2. Data Preprocessing

- Handle missing values (especially in ratings)
- Check for duplicate orders
- Validate data consistency
- Convert data types if necessary

### 3. Univariate Analysis

Analysis of individual variables:

#### Numerical Variables

- **Cost of Order** - Price distribution and spending patterns
- **Food Preparation Time** - How long restaurants take to prepare food
- **Delivery Time** - Time taken for delivery
- **Rating** - Customer satisfaction distribution

#### Categorical Variables

- **Restaurant Name** - Popular restaurants
- **Cuisine Type** - Preferred cuisines
- **Day of the Week** - Weekday vs Weekend order distribution

### 4. Bivariate Analysis

Exploring relationships between variables:

- **Cuisine Type vs Cost**: Which cuisines are most expensive?
- **Day of Week vs Orders**: Weekend vs Weekday patterns
- **Restaurant vs Rating**: Which restaurants have best ratings?
- **Preparation Time vs Rating**: Does prep time affect satisfaction?
- **Delivery Time vs Rating**: Impact of delivery speed on ratings
- **Cost vs Rating**: Relationship between price and satisfaction

### 5. Business Insights Extraction

- Identify top-performing restaurants
- Analyze cuisine preferences
- Understand timing patterns
- Evaluate operational efficiency

---

## ❓ Key Questions to Answer

### Restaurant & Cuisine Analysis

1. **Which restaurants receive the most orders?**
2. **What are the most popular cuisine types?**
3. **How do order costs vary across different restaurants?**
4. **Which cuisines have the highest average order cost?**

### Customer Behavior

5. **What is the distribution of customer ratings?**
6. **How many orders are placed on weekdays vs weekends?**
7. **What is the average order cost per customer?**
8. **Are there repeat customers, and how often do they order?**

### Operational Efficiency

9. **What is the average food preparation time?**
10. **What is the average delivery time?**
11. **Which restaurants have the fastest/slowest preparation times?**
12. **Is there a relationship between preparation time and ratings?**

### Revenue Analysis

13. **What is the total revenue generated?**
14. **Which restaurants contribute most to revenue?**
15. **How does revenue differ between weekdays and weekends?**

---

## 💡 Key Insights & Findings

### Restaurant Performance

- 🏆 **Top Restaurants**: Identify highest-volume restaurants
- ⭐ **Quality Leaders**: Restaurants with best average ratings
- 💰 **Revenue Drivers**: Major contributors to FoodHub revenue

### Cuisine Trends

- 🍕 Most popular cuisine types in New York
- 💵 Price variations across different cuisines
- ⭐ Customer satisfaction by cuisine category

### Timing Patterns

- 📅 **Weekday vs Weekend**: Order volume differences
- ⏰ **Peak Periods**: High-demand time identification
- 📈 **Trends**: Patterns in ordering behavior

### Operational Insights

- ⏱️ **Preparation Efficiency**: Average prep time analysis
- 🚗 **Delivery Performance**: Delivery time patterns
- 📊 **Total Order Time**: Combined prep + delivery analysis

---

## 📈 Visualizations

The analysis includes various visualization types:

| Visualization Type | Purpose                                                   |
| ------------------ | --------------------------------------------------------- |
| **Histograms**     | Distribution of numerical variables (cost, time, ratings) |
| **Bar Charts**     | Restaurant and cuisine comparisons                        |
| **Box Plots**      | Cost and time distribution across categories              |
| **Count Plots**    | Order frequency by day, cuisine, restaurant               |
| **Pie Charts**     | Proportion of weekday vs weekend orders                   |
| **Scatter Plots**  | Relationships between numerical variables                 |
| **Heatmaps**       | Correlation between variables                             |
| **Violin Plots**   | Distribution comparison across groups                     |

---

## 🚀 How to Run

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Steps to Execute

1. Clone or download the repository
2. Navigate to the `food-hub/` directory
3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook foodhub.ipynb
   ```
4. Run all cells sequentially to reproduce the analysis

### Quick Start with Python

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Load the data
foodhub = pd.read_csv('foodhub_order.csv')

# Quick overview
print(foodhub.head())
print(foodhub.info())
print(foodhub.describe())

# View cuisine distribution
plt.figure(figsize=(12, 6))
sns.countplot(y='cuisine_type', data=foodhub, order=foodhub['cuisine_type'].value_counts().index)
plt.title('Order Distribution by Cuisine Type')
plt.xlabel('Number of Orders')
plt.ylabel('Cuisine Type')
plt.tight_layout()
plt.show()

# Analyze ratings distribution
plt.figure(figsize=(10, 6))
sns.histplot(foodhub['rating'].dropna(), bins=10, kde=True)
plt.title('Customer Rating Distribution')
plt.xlabel('Rating')
plt.ylabel('Frequency')
plt.show()
```

---

## 📚 Learning Outcomes

By completing this case study, you will learn:

1. **Exploratory Data Analysis (EDA)**: Comprehensive exploration of business data
2. **Data Visualization**: Creating meaningful charts for business insights
3. **Business Analytics**: Translating data findings into actionable recommendations
4. **Statistical Analysis**: Understanding distributions and relationships
5. **Python Programming**: Practical application of pandas, matplotlib, and seaborn

---

## 🌍 Real-World Relevance

This case study is particularly valuable because:

- **Food Tech Industry**: Understanding dynamics of food delivery platforms
- **Operations Management**: Analyzing preparation and delivery efficiency
- **Customer Experience**: Identifying factors affecting satisfaction
- **Business Strategy**: Data-driven decision making for growth
- **Market Analysis**: Understanding cuisine and restaurant preferences

---

## 📝 Conclusion

This analysis provides FoodHub with:

1. **Demand Understanding**: Clear picture of restaurant and cuisine preferences
2. **Operational Metrics**: Insights into preparation and delivery efficiency
3. **Customer Insights**: Understanding of rating patterns and satisfaction drivers
4. **Revenue Analysis**: Identification of key revenue contributors
5. **Strategic Recommendations**: Data-backed suggestions for business improvement

These findings will enable FoodHub to make informed decisions about restaurant partnerships, customer experience enhancements, and operational optimizations.

---

## 📜 License

This project is for educational purposes.
