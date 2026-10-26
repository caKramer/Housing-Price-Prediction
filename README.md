# Housing-Price-Prediction - R

Utilizes a dataset of housing prices to practice statistical correlation, multiple regression to build a regression model to infer sale price. 

## Includes:

- EDA
  - converted categorical columns to factors
  - checked for missing values
  - checked for duplicates    
- Plotting
  - Scatter plot of price and area
  - histogram for distribution of house prices
  - density plot for property area
  - box plot of price by the categorical variables

## Modeling:

### Linear Regression to predict price based on ‘area’ 

- R^2 = 28.7%
- Intercept: 2,387,000
- Plotted 
  - residuals vs predicted
  - QQ Plot

___

### Linear Regression model using multiple predictor variables to predict sale price

- R^2 = 63.93%
- Intercept: 93,200
- Plotted
  - residuals vs predicted
  - QQ Plot
___

####  Model Comparison

| Metric | Model 1 (Simple: Area) | Model 2 (Multiple) | Statistical Improvement |
| :--- | :--- | :--- | :--- |
| **$R^2$ ($\alpha$)** | 0.2873 | 0.6468 | +125% increase in variance explained |
| **Adjusted $R^2$ ($\beta$)** | 0.286 | 0.6416 | Confirms added variables are meaningful |
| **MSE** | $2.489 \times 10^{12}$ | $1.233 \times 10^{12}$ | ~50% reduction in error variance |
| **RMSE** | $1,577,613$ | $1,110,548$ | Error reduced by approx. $467,000 |

#### ANOVA

| Metric | Model 1 (Simple: Area) | Model 2 (Multiple) | Statistical Improvement |
| :--- | :--- | :--- | :--- |
| **ANOVA ($p$-value)** | Reference Model | $1.249 \times 10^{-77}$ | Highly Significant ($p < 0.05$) |


**Written in R**
