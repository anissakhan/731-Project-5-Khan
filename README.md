# Project 5 - World Wide Products Inc.

### Scope

The dataset used in this project (linked below) contains observations from a variety of products. The products are labeled by a number code only. Each observation also consists of each product's associated warehouse, category code, and date ordered.  The purpose of this project is to use time series models to model and predict the target variable (Product demand, measured by the variable Order_Demand).

### Results

I used Decomposition, SARIMAX, AR, ARMA, and ARIMA models to glean information and form predictions about the demand of a given product. I chose two products (Product 0979 and Product 0704) based on their differing observation counts and distributions. I was able to come up with a relatively accurate forecasting model for Product 0704, but was unable to do so for Product 0979. For Product 0704, the ARIMA model worked best for modeling the data with an MSE of 0.84. The forecasted values, however, were more tenuous.

Please see the Jupyter Notebook for more details and further discussion.

### Data
Datasets obtained from:
1. https://www.kaggle.com/felixzhao/productdemandforecasting


### Variable descriptions

Product_Code - The product name encoded <br />
Warehouse - Warehouse name encoded <br />
Product_Category - Product Category for each Product_Code encoded <br />
Date - The date customer needs the product <br />
Order_Demand - single order qty <br />

### References
1. Dickey-Fuller function definition:
    - https://www.youtube.com/watch?v=McEN54l3EPU
2. To implement ARIMA, ARMA, MA, SARIMAX:
     - https://towardsdatascience.com/machine-learning-part-19-time-series-and-autoregressive-integrated-moving-average-model-arima-c1005347b0d7
     - https://www.geeksforgeeks.org/python-arima-model-for-time-series-forecasting/
2. General Time Series setup in pandas:
    - https://www.dataquest.io/blog/tutorial-time-series-analysis-with-pandas/
    - https://www.datacamp.com/community/tutorials/time-series-analysis-tutorial
