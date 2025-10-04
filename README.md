# Credit Card Consumption Prediction
This project develops a machine learning model to predict future credit card spending based on customer demographics and historical transaction behavior.

### 📈 Business Context and Objective
In the data-rich credit card industry, understanding customer behavior is key to developing effective marketing strategies and improving customer relationships. By analyzing spending patterns, banks can tailor their services and promotions, ultimately boosting sales and revenue. A deep understanding of consumption patterns at an individual level allows banks to customize offerings and make strategic marketing plans.

This project focuses on analyzing and modeling credit card consumption behavior based on customer transaction, demographic, and behavioral data.
The goal was to identify meaningful relationships between features and the target variable, and to build predictive models that could generalize well.
Despite extensive exploration and experimentation, the resulting models performed poorly — with R² scores lower than the **DummyRegressor** baseline.
This indicates that the available features were not sufficiently informative to explain variations in the target variable.

### 🧩 Key Steps in the Notebook
- Data Cleaning: Handling missing values and inconsistent entries.
- Feature Engineering: Identified and removed quasi-constant features
- Exploratory Data Analysis (EDA): Visualizing distributions, correlations, and feature relationships.
- Modeling: Applying various machine learning techniques to predict or classify target outcomes.
- Evaluation: Assessing model performance using standard metrics.

### ⚠️ Results and Limitations
Although many preprocessing and modeling techniques were explored, the final model performance remained less than satisfactory. This is primarily because:
- The dataset’s existing features lack strong predictive signals.
- Many features appear weakly correlated with the target variable.
- The aggregation of consumption data across three months with different day counts (e.g., 28 vs 31 days) makes “average per month” comparisons inconsistent.

### 🚀 Future Work
For future improvement, it is recommended to:
- Transform the target variable to make it more meaningful and consistent — for example, using average credit card usage per day instead of per month.
- Incorporate external data (e.g., calendar events, customer demographics, or macroeconomic indicators) to enrich the dataset.


