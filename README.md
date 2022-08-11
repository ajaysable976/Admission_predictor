# Admission_predictor website 
![website](https://user-images.githubusercontent.com/108600694/184067406-0db971d4-5a1f-4dc1-8ae2-da9c403d67c2.png)

# over-view
Admission Predication is an app used to predict the Chance of Admission(%)

# Model-Steps
- Data has some Missing values(1% to3%) so see the report
- We have used mean as we dont want any data to be removed
- We have Used ALL the feature columns Except Serial no which is of no user for our model
- Scaling down the Feature Varible to normalize(used StandardScaler) the data or to bring all the data to the same range
- We have Used Linear , Ridge (also used RidgeCV) , Lasso((also used LassoCV)) and ElasticNet Regression(also used ElasticNetCV)
- The Score is around 84.2512% to 84.195% and also their adjusted R-Squared(created) but seen that there ans been 2-2.5% decrease in their score
- ALL the Other 3 Models Score and their adjusted was very slightly same
- The score of all model is slightly the same except Elastic , based on my conclusion i have selected Ridge regression as most of the parameter are contributing towards the dependent variable, we would have select Lasso if the vif factor of some are less than 1 as it literaly penalizes the features(if not useful)
- Used the flask server for the deployment 
