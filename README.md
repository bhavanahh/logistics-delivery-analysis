# Delivery Performance Analysis and Strategic Planning in Logistics

## Project Overview

This project focuses on analyzing logistics delivery data to evaluate delivery performance, identify factors associated with delivery delays, and demonstrate how data science can support logistics decision-making.

The project uses a logistics delivery dataset containing 25,000 records and 15 features. The analysis covers data cleaning, exploratory data analysis, KPI calculation, data visualization, correlation analysis, and predictive modeling.

## Problem Statement

Logistics companies need to deliver packages efficiently while minimizing delays and controlling operational costs. Delivery performance can be influenced by factors such as weather conditions, distance, vehicle type, package characteristics, and delivery mode.

The objective of this project is to analyze historical logistics data and identify patterns that can help improve delivery efficiency and support data-driven decision-making.

## Objectives

- Analyze logistics delivery performance.
- Identify factors associated with delivery delays.
- Calculate important logistics performance indicators.
- Explore relationships between logistics variables.
- Visualize delivery performance using Python.
- Build a predictive model for delivery delays.
- Provide strategic recommendations for improving logistics operations.

## Dataset

The project uses a publicly available logistics delivery dataset.

The dataset contains 25,000 delivery records and 15 features, including:

- Delivery Partner
- Package Type
- Vehicle Type
- Delivery Mode
- Region
- Weather Condition
- Distance
- Package Weight
- Delivery Time
- Expected Delivery Time
- Delay Status
- Delivery Status
- Delivery Rating
- Delivery Cost

## Key Performance Indicators

The following KPIs were calculated:

| KPI | Result |
|---|---:|
| Delay Rate | 26.68% |
| Successful Delivery Rate | 73.32% |
| Average Delivery Cost | 864.94 |
| Average Delivery Rating | 3.67 / 5 |

## Methodology

The project follows the following workflow:



Data Collection
      ↓
Data Understanding
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
KPI Calculation
      ↓
Data Visualization
      ↓
Predictive Modeling
      ↓
Model Evaluation
      ↓
Strategic Recommendations


# Exploratory Data Analysis

The analysis examines:

- Delivery status distribution
- Delivery delays under different weather conditions
- Delivery delays across vehicle types
- Relationship between distance and delivery cost
- Delivery performance indicators

### Weather and Delivery Delays

Weather conditions showed a noticeable relationship with delivery delays.

The observed delay rates were:

- **Stormy:** 41.45%
- **Rainy:** 37.35%
- **Foggy:** 30.32%
- **Clear:** 17.43%
- **Hot:** 17.12%
- **Cold:** 16.02%

Stormy weather recorded the highest delay rate.

### Vehicle Type and Delivery Delays

Delay rates across vehicle types were relatively similar, ranging from approximately **26.14% to 27.04%**.

This suggests that vehicle type alone may not be a major factor affecting delivery delays.

### Distance and Delivery Cost

The correlation between distance and delivery cost was approximately **0.99**.

This indicates a very strong positive relationship, meaning that longer delivery distances are strongly associated with higher delivery costs.

## Predictive Modeling

A Logistic Regression model was developed to predict whether a delivery would be delayed.

The target variable was:

```text
delay_target
0 = Not Delayed
1 = Delayed

Categorical variables were converted using **One-Hot Encoding**, while numerical variables were passed directly to the model.

The dataset was divided into:

- **80% training data**
- **20% testing data**

### Model Performance

The Logistic Regression model achieved:

**Accuracy: 89.56%**

This indicates that the model correctly classified approximately 90 out of every 100 delivery records in the test dataset.

## Key Findings

1. Approximately **26.68%** of deliveries were delayed.
2. The successful delivery rate was **73.32%**.
3. The average delivery cost was **864.94**.
4. The average customer rating was **3.67 out of 5**.
5. Stormy weather had the highest delay rate.
6. Rainy and foggy conditions also showed relatively high delay rates.
7. Distance had a very strong positive relationship with delivery cost.
8. Vehicle types showed relatively similar delay rates.
9. Logistic Regression achieved **89.56% accuracy** in predicting delivery delays.

## Strategic Recommendations

- Prepare contingency plans for adverse weather conditions.
- Use predictive analytics to identify deliveries at higher risk of delay.
- Consider delivery distance when planning routes and controlling costs.
- Improve resource allocation based on delivery conditions and requirements.
- Monitor logistics KPIs regularly.
- Incorporate real-time traffic and weather information in future versions.
- Explore advanced route optimization techniques in future work.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Visual Studio Code
- GitHub

## Project Structure

```text
logistics-delivery-analysis/
│
├── data/
│   └── Delivery_Logistics.csv
│
├── notebooks/
│   └── delivery_analysis.ipynb
│
├── README.md
├── requirements.txt
└── Strategic_Planning_Report.docx

## Conclusion

This project demonstrates how data analysis and machine learning can support logistics decision-making. By analyzing delivery performance, weather conditions, distance, costs, and other operational factors, logistics organizations can identify potential problems and develop data-driven strategies to improve efficiency.

The predictive model further demonstrates how machine learning can be used to identify potential delivery delays and support proactive logistics planning.
