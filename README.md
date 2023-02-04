# Regression
Projects based on regression approaches

## Bike Sharing
The main goal is to predict rent (count feature) using the given parameters. The management department will use the results to understand how the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and customer expectations.

I specifically answer which factors contribute most to the number of bicycles checked out over a given day. To answer this question, I build and train a Regression Model on the Capital Bike Share (Washington, D.C.) Kaggle dataset.

### Conclusion
According to EDA:

No specific pattern was observed between a particular day and the number of renting.
On working days, there is a significant rental demand during rush hours.
Regarding the weather, as expected, rainy day has the lowest rent, and the number of renters increased in clear weather.
Fall has the highest rate of ranting esp between 17-18. The high season is from May until October.
There are some correlations between a few features, including atemp and temp, as well as casual and registered. I removed one of the correlated features.
Due to the skewed data distribution, I used the Log value of the target instead of its original value, which could increase the performance by 10% (from 0.39 to 0.49).

Finally, considering the poor R2 score of the trained model, Liner regression is not able to explain the existing non-linearities in the dataset.

Therefore, as a next step, one can further investigate the model in detail by computing the residuals and p-values for different features or using other machine learning approaches.
