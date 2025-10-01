# Advertising-Sales-Analysis

## Objective
This project explores the relationship between advertising expenditures across TV, Radio, and Newspaper media and product sales. It implements data cleaning, exploratory analysis, and linear regression modeling to predict sales based on advertising spend.

## Dataset
The dataset includes 200 advertising campaigns with the following columns:
- **TV**: Advertising expenditure on TV (in thousands)
- **Radio**: Advertising expenditure on Radio (in thousands)
- **Newspaper**: Advertising expenditure on Newspaper (in thousands)
- **Sales**: Resulting product sales (in thousands)

## Data Import & Cleaning
- Dataset contains 200 campaigns
- Missing values in the 'Radio' column are replaced by the column mean
- Data is prepared for analysis and modeling

## Exploratory Analysis
- Average expenditure on TV ads is calculated
- Correlations between advertising channels and sales are examined
- Distribution and relationships between variables are visualized

## Key Questions Addressed
1. **What is the average TV advertising spend?**
2. **How strongly does radio spending correlate with sales?**
3. **Which medium most impacts sales?**

## Regression Modeling
- A linear regression model is built using all advertising channels (TV, Radio, Newspaper) to predict sales
- Model predictions are compared with actual sales values using training/test splits
- Actual vs. predicted sales are visualized with scatter plots for model evaluation

## Feature Impact & Scenario Testing
- Model is used to predict sales for a hypothetical campaign: $200 on TV, $40 on Radio, and $50 on Newspaper
- Effects of normalizing features are tested—normalization greatly improves model performance (R² rises to 0.906)
- Model performance (R² score) drops significantly if only Radio and Newspaper are used as predictors (R² = 0.11 vs. 0.90+ for full-feature model)
- Performance comparison is visualized in a bar chart

## Key Findings
- **TV advertising has the strongest influence on sales** in this dataset
- Linear regression can reasonably predict sales, especially when all features are included
- Data normalization significantly improves model performance
- Model R² score: **0.906** (with normalization and all features)
- Excluding TV as a predictor drastically reduces accuracy to R² = 0.11

## Conclusion
TV advertising has the strongest influence on sales in this dataset. Linear regression can reasonably predict sales, especially when all features are included and data normalization is applied. Excluding TV as a predictor drastically reduces accuracy, highlighting its importance for campaign planning.

## Technologies Used
- Python
- Pandas (Data manipulation)
- NumPy (Numerical computing)
- Scikit-learn (Machine learning and regression modeling)
- Matplotlib/Seaborn (Data visualization)
