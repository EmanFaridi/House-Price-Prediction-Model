##Objective

To build a regression-based machine learning model capable of predicting house prices using numerical housing features.
This task demonstrates key ML skills such as data preprocessing, EDA, model training, evaluation, and visualization.

##Dataset Used

USA Housing Dataset (from Kaggle)
Uploaded manually to Google Colab.
Contains the following features:

Avg Area Income

Avg Area House Age

Avg Area Number of Rooms

Avg Area Number of Bedrooms

Area Population

Address (dropped during preprocessing)

Price (target column)

##Data Preprocessing Steps

To prepare the dataset for training, the following steps were performed:

Loaded the CSV dataset into pandas

Inspected dataset structure using .info(), .describe(), and .head()

Verified dataset shape and column types

Removed non-numeric fields such as Address

Checked and handled missing values (none or filled using median)

Split dataset into features (X) and target (y)

Applied train-test split (80% training, 20% testing)

Scaled numerical features using StandardScaler
##Exploratory Data Analysis (EDA)

Performed visual analysis to understand relationships in the dataset:

Correlation Heatmap
Displayed relationships between numerical features

Price Distribution Plot
Helped understand target variable spread

Scatter Plot: Actual vs Predicted Prices
Evaluated model performance visually

##Models Applied

Two regression models were implemented and tested:

##Linear Regression

Served as the baseline model

Performed well with standardized numerical features

Gradient Boosting Regressor (optional, tested for comparison)

More powerful non-linear model

Typically offers improved prediction accuracy

##Model Evaluation

The model was evaluated using:

MAE (Mean Absolute Error)
Measures average distance between predicted and actual values

RMSE (Root Mean Squared Error)
Penalizes larger errors more than MAE

These metrics provided a balanced performance assessment of the prediction model.

##Key Findings & Insights

Strong correlations were observed between population, income levels, and house prices

House age and room counts also contributed to price variations

Removing irrelevant text-based fields such as Address improved model performance

Standardizing features significantly improved regression output

The regression model performed reliably, predicting prices with reasonable accuracy

##Repository Contents

house_price.ipynb — Complete Google Colab notebook

USA_Housing.csv — Dataset used

README.md — Documentation file (this file)

##Tools & Libraries Used

Python 3

pandas, numpy — Data manipulation

matplotlib, seaborn — Visualizations

scikit-learn — Model training & evaluation

Google Colab — Development environment

##Conclusion

This project provided a complete machine learning workflow for predicting house prices.
The task demonstrated:

Data loading & preprocessing

EDA for feature understanding

Regression model development

Error-based evaluation

Visual comparison of predictions vs real values

The model successfully predicts house prices and establishes a foundation for more advanced regression tasks.