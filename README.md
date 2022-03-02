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

<img width="1114" alt="Screen Shot 2022-02-24 at 23 23 55" src="https://user-images.githubusercontent.com/86486485/155641816-792e1197-5594-4281-96e3-3816a1b343c9.png">

<img width="1111" alt="Screen Shot 2022-02-24 at 23 25 03" src="https://user-images.githubusercontent.com/86486485/155641907-90f8cd78-6196-4ddc-bd73-28a4b2137d35.png">

**Feature Selection**: split dataset and Boruta Algorithm.

**Machine Learning Modelling**: machine learning model training.

**Convert Model Performance to Business Values**: deliver a dataset with the worst and best scenario, MAPE ana MAE scores.

# 4. Top 3 Data Insights

**H1.** Stores with greater assortment should sell more.

**H1. Validation = False:** Stores with greater assortment sell less.
<img width="1107" alt="Screen Shot 2022-02-24 at 23 18 05" src="https://user-images.githubusercontent.com/86486485/155641561-a53e93e0-9f6d-40c0-bdf9-28e93dd94642.png">

**H2.** Stores with close competitors should sell less.

**H2. Validation = False:** Stores with close competitors sell more.
<img width="1119" alt="Screen Shot 2022-02-24 at 23 19 43" src="https://user-images.githubusercontent.com/86486485/155641358-a874d107-cde1-40fa-bb7f-478542ea0089.png">

**H7.** During Chirstmas, stores should sell more.

**H7. Validation = False:** During Chirstmas holiday, stores sell less.
<img width="1122" alt="Screen Shot 2022-02-24 at 23 20 26" src="https://user-images.githubusercontent.com/86486485/155641598-29edaaac-90bd-4cdc-971c-e3257f31f534.png">


# 5. Machine Learning Model Applied
- Average Model
- Linear Regression Model
- Linear Regression Regularized Model (Lasso)
- Random Forest Regressor

# 6. Machine Learning Modelo Performance
## **Final Model:** Random Forest Regressor

<img width="475" alt="Screen Shot 2022-02-24 at 22 59 28" src="https://user-images.githubusercontent.com/86486485/155639524-48009d57-3193-4ab1-b051-6507e96ac712.png">

# 7. Business Result

<img width="1118" alt="Screen Shot 2022-02-24 at 23 26 06" src="https://user-images.githubusercontent.com/86486485/155642137-7f353826-75c2-41a5-bf6e-6fb685c6bb40.png">

# 8. Conclusions
This is the first CRISP-DS cycle. The predective model presents a useful performance, but there are stores with a higher MAPE, requiring another modeling strategy. In the next CRISP-DS cycle this point should be improved.

**Business Performance**
![image](https://user-images.githubusercontent.com/86486485/156441147-fc495fb5-a63b-4e9d-b867-60f30fabdcd3.png)

**Total Performance**
![image](https://user-images.githubusercontent.com/86486485/156441654-96089628-a842-49cc-a692-abacb5e86825.png)



# 10. Next Steps to Improve
Treat the problem with XGboost algorithm.

# All Rights Reserved - Comunidade DS 2021
