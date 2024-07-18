# Stock_Price_Machine_Learning_Project
##Creating a machine learning model to predict future stock price. 
### Collaborators
    * 

## Project Synopsis

### Overview
This project focuses on analyzing and preparing data related to Amazon stock (ticker symbol: AMZN) for further modeling and analysis. The dataset includes minute-level stock prices and various technical indicators obtained from Yahoo Finance.

### Key Components

#### Data Collection and Integration
- **Yahoo Finance API Integration:** Utilizes the Yahoo Finance API to fetch minute-level stock prices (open, high, low, close) and technical indicators such as Simple Moving Averages (SMA).
- **Additional Financial Data:** Retrieves essential company financials including revenue, net income, gross profit, total debt, and operating cash flow from Yahoo Finance for comprehensive analysis.

#### Data Cleaning and Preprocessing
- **Handling Missing Values:** Implements appropriate methods to handle missing values, utilizing mean imputation for technical indicators like 'QQEs_14_5_4.236' and median imputation for other metrics to maintain data integrity.
- **Outlier Detection and Treatment:** Detects outliers using the Interquartile Range (IQR) method and applies Windsorization to cap extreme values, ensuring robustness in subsequent analyses.

#### Statistical Analysis
- **KS Test for Distribution Comparison:** Utilizes the Kolmogorov-Smirnov (KS) test to compare the distributions of selected technical indicators against the closing price of Amazon stock, providing insights into their relationship and potential predictive power.
- **Principal Component Analysis (PCA):** Performs PCA to reduce dimensionality and identify principal components that explain significant variance in the dataset. After analysis:
  - Retaining 90% of variance reduces features to 20 components.
  - Retaining 95% of variance reduces features to 34 components.
  - Retaining 99% of variance reduces features to 60 components.
  - Further analysis explores the overlap and significance of these components to refine feature selection.

#### Visualization
- **Moving Averages Analysis:** Visualizes various Simple Moving Averages (SMA) against the closing price to assess their effectiveness in smoothing out noise and identifying underlying trends in Amazon stock price movements.

#### Model Preparation Considerations
- **Feature Engineering:** Engineers new features derived from technical indicators and financial metrics to enhance the dataset's predictive capabilities for modeling purposes.
- **Data Integrity Checks:** Ensures data quality through rigorous cleaning, validation, and verification processes before applying predictive models.

### Conclusion
This project aims to provide a comprehensive understanding of Amazon stock dynamics through rigorous data analysis and preparation. By integrating minute-level stock prices, financial data, and technical indicators, and applying statistical tests, PCA, and visualization techniques, it lays the groundwork for developing robust predictive models. The insights gained from this analysis are intended to support informed decision-making processes related to Amazon stock investments and market strategies.
