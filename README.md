# Rossmann-Store-Sales
Project from Data Science Community, mentoring by Meigarom Lopes. This repository contains script that predicts the next customer purchase using a Time Series approach.

**Dataset**: https://www.kaggle.com/c/rossmann-store-sales

# 1. Business Problem
Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.

# 2. Business Assumptions
- The CFO has problems to setting the budget and making decisions.
- Stores do not have Competition Distance information, the assumptions was that the distance should be the greatest distance observed in the dataset.
- Managers do not uniformly apply sales forecasting.
- A predictive sales model for all stores.

# 3. Solution Strategy
My strategy to solve this challenge was:

**Data Description**: descriptive analysis to identify outliers and to provide metrics such as mean, median, maximum, minimum, range, skew, curtosis and standard deviation. Cheeck and fillout NA.

**Feature Engineering**: create new attributes based on the original variables using mindmap hypothesis.

**Exploratory Data Analysis**: univariate, bivariate and multivariate analysis with numerical and categorical variables.

**Feature Selection**: split dataset and Boruta Algorithm.

**Machine Learning Modelling**: machine learning model training.

**Convert Model Performance to Business Values**: deliver a dataset with the worst and best scenario, MAPE ana MAE scores.

# 4. Top 3 Data Insights

**H1.** Stores with greater assortment should sell more.

**H1. Validation = False:** Stores with greater assortment sell less.

**H2.** Stores with close competitors should sell less.

**H2. Validation = False:** Stores with close competitors sell more.

**H7.** During Chirstmas, stores should sell more.

**H7. Validation = False:** During Chirstmas holiday, stores sell less.

# 5. Machine Learning Model Applied
- Average Model
- Linear Regression Model
- Linear Regression Regularized Model (Lasso)
- Random Forest Regressor

# 6. Machine Learning Modelo Performance
<img width="475" alt="Screen Shot 2022-02-24 at 22 59 28" src="https://user-images.githubusercontent.com/86486485/155639524-48009d57-3193-4ab1-b051-6507e96ac712.png">

<img width="475" alt="Screen Shot 2022-02-24 at 22 59 28" src="https://user-images.githubusercontent.com/86486485/155639524-48009d57-3193-4ab1-b051-6507e96ac712.png">

# 7. Business Results
<img width="475" alt="Screen Shot 2022-02-24 at 22 59 28" src="https://user-images.githubusercontent.com/86486485/155639524-48009d57-3193-4ab1-b051-6507e96ac712.png">

# 8. Conclusions
This is the first CRISP-DS cycle. The predective model presents a useful performance, but there are stores with a higher MAPE, requiring another modeling strategy. In the next CRISP-DS cycle this point should be improved.

# 10. Next Steps to Improve
Treat the problem with XGboost algorithm.

# All Rights Reserved - Comunidade DS 2021
