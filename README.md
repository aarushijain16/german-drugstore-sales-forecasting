# german-drugstore-sales-forecasting
Implemented robust Machine Learning models to accurately forecast sales for a German drugstore chain, providing actionable predictions to optimize inventory and operational planning.
# German Drugstore's Retail Sales Forecasting 
## Executive Summary:
This project focuses on providing accurate future sales predictions for a German drugstore chain and gaining insights into the variables influencing those sales. Leveraging advanced machine learning techniques, the analysis identifies key factors affecting sales performance, enabling data-driven strategic decsions for improved sales in various store contexts. 

## Problem Statement:
The primary aim of this report was to equip a German drugstore chain with:
* **Accurate Sales Predictions**: To forecast future retail sales to aid in strategic planning, inventory management, and resource allocation.
* **Understanding Influencing Variables**: To identify and analyse the key factors that drive sales, such as store type, assortment, state holidays, day of the week, and promotional activities.

## Data Sources and Confidentaility:
The analysis was conducted using a proprietary dataset from a German drugstore chain. Due to the confidential nature of this dataset, it **cannot be shared publicly** in this repository.

The dataset contained detailed retail sales information, including historical sales figures, customer counts, store-specific attributes (e.g., store type, assortment), calendar-related features (e.g., date, day of week, state holidays, school holidays), and promotional indicators. 

## Methodology:
This project employed a robust machine learning-driven approach to sales forecasting:
* **Exploratory Data Analysis (EDA)**:
  * Initial EDA was performed to understand data distributions and identify initial relationships.
  * Analysis showed that average sales and customers vary significantly by store type, assortment type, state holidays, and day of the week.
    
* **Data Preprocessing and Feature Engineering**:
  * Data was prepared for machine learning, including handling missing values, encoding categorical features, and creating new time-based features (e.g., month, year, day of week, day of year).

* **Clustering for Model Optimisation**:
  * The data was intelligently clustered:
     * **Initial Clustering**: Store types with distinctly different average sales and customer patterns were initially separated, while similar store types were grouped together.
     * **Sub-Clustering**: Within these initial clusters, further sub-clusters were created based on seasonality, after determining the ideal number of clusters for each group.
     * The purpose of this clustering was to compare and apply the best-performing predictive model for each specific cluster, optimizing overall forecasting accuracy.
* **Predictive Modelling (Machine Learning)**:
  * **Random Forest Regressor**: This ensemble learning method was applied and found to provide the most accurate predictions for sales forecasting.
  * **Multilayer Perceptron (MLP) Regressor**: An Artificial Neural Network model was also attempted as part of the predictive analysis.
    * Model performance was rigorously evaluated across all clusters, ensuring the best-performing model was selected for each segment.
  * **Analysis of Influencing Factors**: Further analysis was explored to identify other variables affecting sales, such as pricing strategies and marketing campaigns.

## Key Findings and Impact:
* **Variable Impact on Sales**: Demonstrated that sales and customer numbers are significantly influenced by variables such as store type, assortment, state holidays, and day of week.
* **Effective Promotional Strategies**: Analysis of promotional activities (Promo, Promo2( through boxplots showed their varying imapct on sales and customer numbers.
* **School Holiday Influence**: Identified the impact of school holidays on sales and customer behaviour.
* **Optimised Forecasting**: The use of a clustered modelling approach (with Random Forest as the best performer) yielded accurate sales forecasts, enabling the drugstore chain to make more informed business decisions.
* **Actionable Recommendations**: The insights provided direct recommendations to focus promotions and advertising efforts strategically, particularly in areas or contexts (e.g., store types, days) categorised by lower historical sales. This aimed to increase overall sales and gain deeper insights into customer purchasing patterns and demand for different assortments.

## Tools and Technologies:
* **Machine Learning Libraries**: Scikit-learn for Random Forest nd MLP regressor (as implied by standard Python ML workflows).
* **Programming Languages**: Python (for ML), SAS Enterprise Guide and Excel (for data manipulation).
* **Data Analysis Libraries**: Pandas, NumPy (for data manipulation).
* **Data Visualisation Libraries**: Matplotlib, Seaborn (for creating informative plots like boxplots mentioned in the appendix).

## Confidentiality Note:
Due to the confidential nature of the dataset and the analysis performed for the German drugstore chain, **the raw data and the project code cannot be shared publiclu** in this repository. This 'README.md' serves to outline the problem, methodology, and key findings of the project. 

## Visualisations:
