# Ames Housing Data
##### created by: Rex Chang

#### Contents:
- [Problem Statement](#Problem-Statement%3A)
- [Brief Data Describtion](#What-kind-of-data-are-we-dealing-with-%3F)
- [Conclusion](#Conclusion%3A)

## Problem Statement:
---
When it comes to searching for new house, ask a home buyer to describe their dream house, and they probably won't begin with, rather or not if the garage is attached to the house or the square feet of second floor. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, I will use different methods in machine learning and select the one that can produce the most accurate prediction.


Our objective is to assist the clients to find out what are the features that actually impact the housing price the most in Ames, Iowa. I will perform EDA on the dataset and then apply to the three regression models: Linear Regression, Lasso, and Ridge. Then we observe and select the model that produce the lowest RMSE and highest R^2 to obtain the top 25 features. After discovering the 25 important features that impact the house price the most. We can generate and predict the house price for our clients to compare with the house price lists/asked by the seller to see if they're getting a reasonable price before buying the house.

---
## Libraries/model used:
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- Lasso
- Linear Regression
- Rigde

### What kind of data are we dealing with ?
The Ames Housing Dataset is a really detailed dataset with appoximately 79 columns of different features relating to houses. first step is to perform an exploratory data analysis, cleaning the data.

The Ames Housing Dataset is an exceptionally detailed and robust dataset with over 70 columns of different features relating to houses. While the two models predicted different targets (and required different features, model choices, and hyperparameters), I was able to use the rich knowledge I developed from generating one model to help inform the other.

Data Describtion can be found [Here](https://www.kaggle.com/c/dsi-us-6-project-2-regression-challenge/data)

## Conclusions and Recommendations
---

| feature | weight |
| --- | --- |
| overall_qual | 1.62e+04 |
| gr_liv_area | 1.16e+04 |
| 2nd_flr_sf | 8.75e+03 |
| garage_type_Attchd | 7.59e+03 |
| garage_area | 7.18e+03 |
| kitchen_qual_Ex | 7.14e+03 |
| neighborhood_NridgHt | 6.17e+03 |
| fireplaces | 6.13e+03 |
| neighborhood_NoRidge | 5.57e+03 |
| mas_vnr_type_None | 5.50e+03 |
| garage_type_Detchd | 5.41e+03 |
| year_remod/add | 5.04e+03 |
| ms_zoning_RM | -4.93e+03 |
| total_bsmt_sf | 4.77e+03 |
| 1st_flr_sf | 4.73e+03 |
| exter_qual_Ex | 4.72e+03 |
| lot_area | 4.71e+03 |
| bsmt_exposure_Gd | 4.67e+03 |
| bsmt_qual_Ex | 4.62e+03 |
| neighborhood_StoneBr | 4.31e+03 |
| mas_vnr_type_BrkFace | 4.11e+03 |
| garage_type_BuiltIn | 3.92e+03 |
| bsmtfin_sf_1 | 3.56e+03 |
| sale_type_New | 3.44e+03 |
| year_built | 3.18e+03 |

### Conclusion:
In conclusion, after refining our models over time, and the use of train-test split, cross-validation, and cleaning data with unknown values for the target to simulate the model process, with the final dicision of using Ridge Regression, we have conduced the top 25 features that impact the most to our housing price in Ames, Iowa. Now, we can predict the house price depending on those 25 features then assist our clients that are actively searching for house in Ames to see if the asked price is reasonable.

My recommendation for this case is, if given more time to gather more detailed informations, we can predict and compare better modeling result for house price in Ames. For example, gather true housing data from local cities near Ames (like [Ankeny](https://www.zillow.com/ankeny-ia/home-values/)) to compare and/or gather data that represents how the true housing price changed overtime to forcast the house price in near future (somethinge like [This](https://www.zillow.com/ames-ia/home-values/)). With better modeling result that we can provide to our clients, this will not only create higher revenue but also beneficial to the company’s reputation.