# Red Wine Quality Analysis Project 
# Overview
This project builds a machine learning model to predict the quality of red wine based on its various chemical attributes, such as acidity, sugar content, pH, alcohol percentage, and more. 
# Data Description
The analysis is based on the following attributes in the dataset: 
* **Fixed Acidity:** The amount of tartaric acid in the wine (g/dm³).
* **Volatile Acidity:** The amount of acetic acid in the wine (g/dm³).
* **Citric Acid:** The amount of citric acid in the wine (g/dm³).
* **Residual Sugar:** The amount of residual sugar in the wine (g/dm³).
* **Chlorides:** The amount of chlorides in the wine (g/dm³).
* **Free Sulfur Dioxide:** The amount of free sulfur dioxide (mg/dm³).
* **Total Sulfur Dioxide:** The total amount of sulfur dioxide (mg/dm³).
* **Density:** The density of the wine (g/cm³).
* **pH:** The pH of the wine.
* **Sulphates:** The amount of sulfates in the wine (g/dm³).
* **Alcohol:** The alcohol content of the wine (%).
* **Quality:** The quality rating of the wine (on a scale from 3 to 8, with higher values indicating better quality).
# Methodology  
1. Remove duplicates and ensure data integrity (no missing values or invalid entries) within the dataset 
2. Analyze key correlations between chemical attributes (such as acidity, sulfur dioxide) and wine quality. Visualize relationships using **heatmaps** and **histograms** to identify patterns.
3. Train a Linear Regression model to predict wine quality based on relevant features, using an **80-20 test split**.
4.  Evaluate the model's performance using metrics including **Mean Squared Error (MSE)**, **R^2**, and **Mean Absolute Percentage Error (MAPE)**. Apply thresholding to round predictions to the nearest quality score (integer).
5.  Analyze the model's performance and key impacts (such as alcohol, acidity) to offer actionable insights into wine quality improvement strategies.  
# Results 
1. **Correlations Analysis:** High alcohol content is strongly positively correlated with better wine quality, while volatile acidity is negatively correlated with wine quality.
2. **Model Performance:** The Linear Regression model performs adequately for the given dataset, but other models such as Random Forest could improve performance by capturing more complex relationships.
3. **Error Metrics:** The Mean Absolute Percentage Error (MAPE) is below 10% for both training and testing data, which indicates a good fit for the model. Residual analysis shows minimal error, confirming that the model is performing well. 
# Technologies Used 
* **Pandas & NumPy:** For data manipulation, cleaning, and handling numerical operations.
* **Matplotlib & Seaborn:** For data visualization and creating insightful plots (e.g., heatmaps, histograms).
* **Scikit-learn:** For machine learning model development, training, and evaluation.
# Future Developments 
* Implement and compare additional machine learning models(such as Random Forest or Gradient Boosting) to improve prediction accuracy.
* Develop an interactive dashboard using tools such as Tableau to visualize key wine quality trends, model performance metrics, and feature impacts.
* Create a real-time prediction feature with Streamlit, allowing users to input chemical attributes and predict wine quality instantly.
