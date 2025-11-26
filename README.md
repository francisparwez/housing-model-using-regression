# housing-model-using-regression

✅ SECTION 1 — Importing Required Libraries (Description)

In this section, we import all the essential Python libraries used for data analysis, visualization, and model building:

NumPy & Pandas — for numerical operations and data manipulation.

Matplotlib & Seaborn — for plotting graphs and visualizing relationships between features.

Scikit-learn tools — 

fetch_california_housing() to load the dataset,

train_test_split() to split data into training and test sets,

evaluation metrics such as R² score and Mean Absolute Error.

XGBoost Regressor — a powerful gradient boosting model used to build the regression model.

This section essentially sets up the entire environment needed for data preprocessing, analysis, visualization, and machine learning.

✅ SECTION 2 — Loading and Inspecting the Dataset (Description)

In this section, we load the California Housing dataset. 

After loading:

The dataset is converted into a Pandas DataFrame using its feature names.

The target variable (median house value) is appended to the DataFrame.

We display:

the first few rows (head()) to understand the structure,

the dataset shape (rows & columns),

and the count of missing values.

This helps verify that the dataset loaded correctly and ensures that we have complete, clean data before moving forward with modeling.

✅ SECTION 3 — Statistical Summary & Correlation Analysis (Description)

In this section, we perform exploratory data analysis (EDA):

📊 Descriptive Statistics

Using df.describe(), we generate statistical summaries (mean, median, standard deviation, quartiles) for every feature.
This helps us understand:

Data distribution

Feature ranges

Possible outliers

🔗 Correlation Matrix

We compute the correlation matrix to identify how strongly each feature is related to the target variable and to each other.

🔥 Correlation Heatmap

A heatmap is plotted using Seaborn to visualize these relationships.
This makes it easy to:

Spot highly correlated features,

Detect redundant predictors,

Understand which features may influence the house price the most.

This EDA step is crucial before training a machine learning model, as it gives insight into data patterns and helps guide feature selection.