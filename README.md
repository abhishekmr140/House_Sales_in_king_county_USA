📋 Project Context: 
In this project, I acted as a Data Analyst for a Real Estate Investment Trust (REIT). The organization aimed to expand its portfolio into residential real estate. My objective was to develop a data-driven model to accurately estimate market prices in King County, USA, based on property attributes like square footage, location, and structural features.

🧪 Technical Implementation: 
The project follows a rigorous data science workflow across several key stages:
Data Acquisition & Cleaning: Handled a dataset of 21,613 observations, managing missing values for bedroom and bathroom counts to ensure data integrity.
Exploratory Data Analysis (EDA): Utilized Seaborn and Matplotlib to visualize correlations (e.g., waterfront views vs. price) and determine the most influential features.
Feature Engineering: Applied Polynomial Transformations to capture non-linear trends in housing data.
Model Pipeline: Developed a scikit-learn Pipeline object to automate:
Data Scaling (StandardScaler)
Polynomial Feature Generation
Linear Regression Modeling
Regularization: Implemented Ridge Regression to mitigate overfitting, optimizing the model's performance on validation data.

🎯 Business Impact: 
The final model provides the REIT with a systematic way to identify undervalued properties and predict the ROI of potential acquisitions, moving from "gut-feeling" estimates to evidence-based valuation.
