# Food Sales Predictions
## Using different variables to predict food sales in stores

**Alexander Re** 

### Business problem:

How do variables such as Item Type, Visibility, Outlet Type, and Outlet Size impact the sale of items in a store?


### Data Source: 
https://datahack.analyticsvidhya.com/contest/practice-problem-big-mart-sales-iii/


## To prepare this data, the data was cleaned, and the following processes were performed:


### Explanatory Data Analysis
#### - A histogram was used to determine the distribution of Item Outlet Sales.
#### - Histograms and boxplots were used on all categorical data.
![](Screen%20Shot%202023-02-02%20at%2010.07.23%20PM.png)
> The histogram shows that the majority of sales were around 2000 rupees.


### Exploratory Data Analysis
#### - This bar graph shows the mean amount of sales for each outlet type.
![](Screen%20Shot%202023-02-02%20at%209.54.34%20PM.png)
> Supermarket Type 3 had the highest amount of sales, with an average of over 3,500 rupees.
> Grocery Stores had the lowest amount of sales, with an average of just under 500 rupees. 

#### - This bar graph shows the average sales for each item type. 
![](Screen%20Shot%202023-02-02%20at%209.54.21%20PM.png)
> By a small margin, starchy foods had the most sales, with an average of 2,500 rupees.
> Three of the lowest selling item types were baking goods, soft drinks, and a category listed as "other."

## Model

The model used was a Decision Tree Regression Model. 

### Important metrics
#### Train
- MAE: 762.610
- MSE: 1172122.773
- RMSE: 1082.646
- R2: 0.603
#### Test
- MAE: 738.317
- MSE: 1118185.97
- RMSE: 1057.443
- R2: 0.594

>This model performed relatively well, with an R2 score of 0.603 for the train data and 0.594 for the test data. Because the R2 values are close together, the model has a low variance. 

#### LinearRegressions Coefficients
![](Food-Sales-Predictions/blob/main/lin_reg_coefficients.png)

#### RandomForest Importances
![](Food-Sales-Predictions/blob/main/rf_importances.png)



## Recommendations:

Based on the exploratory data, I reccommend that more resources should be allocated towards Type 3 Supermarkets, as they provide the most amount of value out of all store types. I would also reccommend that more effort should be put into advertising soft drinks and baking goods, in order to increase sales. These were some of the lowest selling items. 

## Limitations & Next Steps

This data can be used to help understand what can be improved in each store. For example, after viewing the low sales of grocery stores, more data can be collected on why they are doing so poorly. After collecting this data, steps can be taken to help mitigate the issues. 
