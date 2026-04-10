# House Price Prediction using Linear Regression

## Overview
This project focuses on predicting median house values using various features from a housing dataset (such as Average Rooms, Crime Rate, Property Tax Rate, etc.). A **Linear Regression** model is implemented to understand the relationship between these features and the target variable (`Median_Home_Value`).

## Objective
* **Data Exploration:** Analyze correlations between features and the target variable using a correlation matrix and seaborn heatmap.
* **Model Training:** Train a Linear Regression model on the labeled housing dataset.
* **Evaluation:** Evaluate the model's performance on the training data using **Root Mean Squared Error (RMSE)**.
* **Feature Importance:** Extract and interpret the model coefficients to determine which features have the most significant impact on housing prices.

## Dataset
The project uses the **House Prediction Data Set** (`dataset/house_Prediction_Data_Set.csv`), which includes features such as:
* `Average_Rooms` (Number of rooms per dwelling)
* `Crime_Rate` (Per capita crime rate by town)
* `Nitric_Oxide_Concentration` (Nitric oxides concentration)
* `Lower_Status_Pop_Percent` (% lower status of the population)
* *...and other relevant housing metrics.*

## Key Findings
* **Correlation:** Features like `Average_Rooms` show a strong positive correlation with the median home value, while `Lower_Status_Pop_Percent` shows a strong negative correlation.
* **Model RMSE:** The Linear Regression model achieved an RMSE of approximately **4.65** on the training data.
* **Model Coefficients:** The coefficients reveal that `Average_Rooms` has the highest positive coefficient (increasing home value), while `Nitric_Oxide_Concentration` and `Distance_To_Work_Centers` have negative coefficients (decreasing home value).

## Project Structure
* `main.ipynb`: The Jupyter Notebook containing the data exploration, model training, and evaluation code.
* `dataset/house_Prediction_Data_Set.csv`: The dataset used for training the model.
* `README.md`: Project documentation.

## Requirements
* Python 3.x
* Pandas
* NumPy
* Matplotlib & Seaborn (for data visualization)
* Scikit-Learn (for model training and evaluation)

## Getting Started
1. Install the required libraries using `pip install pandas numpy matplotlib seaborn scikit-learn`.
2. Open `main.ipynb` in a Jupyter environment.
3. Run the cells sequentially to observe data preprocessing, exploratory data analysis, and the Linear Regression results.
