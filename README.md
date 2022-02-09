# House Price Prediction
### Problem Statement
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia.


## Table of Contents
* [Objective](#objective)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

<!-- You can include any other section that is pertinent to your problem -->

### Objective

* Which variables are significant in predicting the price of a house, and

* How well those variables describe the price of a house.

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.


## Conclusions
Lasso Regression outperformed others.

| Metric           | LinearRegression() | Ridge(alpha=2.0) | Lasso(alpha=0.001) |
| :--------------- | :----------------- | :--------------- | ------------------ |
| R2 Score (Train) | 9.547200e-01       | 0.93727          | 0.91020            |
| R2 Score (Test)  | -3.084162e+20      | 0.89662          | 0.89268            |
| RSS (Train)      | 6.573600e+00       | 9.10616          | 13.03574           |
| RSS (Test)       | 2.702579e+22       | 9.05861          | 9.40408            |
| MSE (Train)      | 6.720000e-03       | 0.00931          | 0.01333            |
| MSE (Test)       | 5.607011e+19       | 0.01879          | 0.01951            |

The Top Predictor variables from Lasso and Ridge are:
  - Lasso Regression `Lasso(alpha=0.001)`
    - Top 5 Features
      1. GrLivArea
      2. building_remod_age
      3. OverallQual
      4. 1stFlrSF
      5. LotArea
   
- Ridge Regression `Ridge(alpha=2.0)`
    - Top Positive Coefficients
        1. GrLivArea
        2. 1stFlrSF
        3. LotArea
        4. OverallQual
        5. 2ndFlrSF


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.8.9
- Requirements file contents
  - python = "^3.8"
  - jupyter = "^1.0.0"
  - pandas = "^1.4.0"
  - sklearn = "^0.0"
  - numpy = "^1.22.1"
  - matplotlib = "^3.5.1"
  - plotly = "^5.5.0"
  - seaborn = "^0.11.2"
  - pyarrow = "^6.0.1"
  - Flask = "^2.0.2"
  - pandas-profiling = "^3.1.0"
  - sweetviz = "^2.1.3"
  - dash = "^2.1.0"
  - jupyter-dash = "^0.4.0"
  - scikit-learn = "1.0.1"
  - statsmodels = "^0.13.1"

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->



## Contact
Created by [@Vinay26k](https://github.com/Vinay26k) - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
