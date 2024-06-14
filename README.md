# EV Market Segmentation Analysis

## Overview
This project focuses on analyzing the Electric Vehicle (EV) market in India using segmentation analysis. The primary goal is to develop a feasible strategy for an EV startup to enter the market by targeting segments that are most likely to adopt electric vehicles. The analysis involves examining consumer buying behavior, demographic factors, and geographic data, followed by clustering analysis to identify distinct consumer segments.

## Table of Contents
- [Introduction](#introduction)
- [Data Preprocessing](#data-preprocessing)
- [Behavioral and Psychographic Analysis](#behavioral-and-psychographic-analysis)
- [Demographic Analysis](#demographic-analysis)
- [Geographic Analysis](#geographic-analysis)
- [Model Implementation](#model-implementation)
- [Conclusion](#conclusion)
- [How to Run the Project](#how-to-run-the-project)

## Introduction
Understanding the EV market dynamics in India is crucial for developing effective marketing and business strategies. This analysis provides insights into various factors influencing consumer behavior and preferences for electric vehicles, helping identify key market segments.

## Data Preprocessing
The initial steps involve loading and inspecting the data to ensure its quality and readiness for analysis.

1. **Import Libraries**:
   - Import necessary libraries for data manipulation, visualization, and machine learning.

2. **Load Dataset**:
   - Load the consumer buying behavior dataset (`MARKET_BEHAVIOUR_ANALYSIS.csv`).

3. **Inspect Data**:
   - Check the dataset for null values and ensure data consistency.
   - Print unique values for categorical columns to understand the data better.

4. **Data Cleaning**:
   - Replace inconsistent entries (e.g., replace 'm' with 'No' for the 'Wife Working' column).

## Behavioral and Psychographic Analysis
Visualize and analyze the relationships between consumer demographics and their vehicle purchase behaviors.

- **Age**: Younger consumers tend to purchase less expensive vehicles.
- **Number of Dependents**: Consumers with more dependents prefer vehicles with more seats, such as SUVs.
- **Salary**: There is a direct relationship between salary and the price of the vehicle purchased.

Visualizations include:
- Violin plots to observe the distribution of various features against the 'Make' of vehicles.
- Scatter plots and count plots to understand the relationship between consumer demographics and vehicle preferences.

## Demographic Analysis
Analyze the distribution of key demographic features such as age, number of dependents, salary, and vehicle price.

- **Age Distribution**: Most consumers are between 25 and 50 years old.
- **Total Salary Distribution**: Consumers with an average total salary of around 30 lakhs tend to purchase vehicles more.
- **Price Distribution**: Most vehicles purchased fall within the 10 to 20 lakh price range.

## Geographic Analysis
Analyze the state-wise sales data to identify regions with higher adoption rates of electric vehicles.

- Load and visualize state-wise EV sales data (`EV_DATA.csv`).
- Identify top states for each category of electric vehicles.
- Target states with higher numbers of EVs for marketing and sales efforts.

## Model Implementation
Use K-Means clustering to segment consumers based on various features.

1. **Data Preparation**:
   - Encode categorical variables.
   - Standardize the features for clustering.

2. **Determine Optimal Number of Clusters**:
   - Use the Elbow Method to find the optimal number of clusters.

3. **K-Means Clustering**:
   - Implement K-Means clustering with the optimal number of clusters.
   - Visualize the clusters to understand distinct consumer segments.

## Conclusion
The analysis provides a comprehensive understanding of the EV market in India, highlighting key factors influencing consumer behavior and preferences. The clustering analysis helps identify distinct consumer segments, enabling the startup to target the most promising market segments effectively.

## How to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/EV_Market_Segmentation_Analysis.git
   cd EV_Market_Segmentation_Analysis
   ```

2. **Install Dependencies**:
   - Ensure you have Python installed.
   - Install necessary packages:
     ```bash
     pip install pandas numpy matplotlib seaborn scikit-learn
     ```

3. **Run the Analysis**:
   - Execute the Jupyter notebook or Python script containing the analysis.

4. **Review the Results**:
   - Inspect the visualizations and model outputs to understand the insights and conclusions drawn from the analysis.

---

This README file provides a structured overview of the project, helping users understand the objectives, methodologies, and outcomes of the EV market segmentation analysis.
