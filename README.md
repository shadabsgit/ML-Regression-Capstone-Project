# Seoul Bike Sharing Demand Prediction
Currently many big cities have adopted the use of rental bikes to improve mobility comfort. It is crucial to make the rental bikes accessible and available to the general public at the appropriate time since it reduces waiting. Eventually, maintaining a steady supply of rental bikes for the city emerges as a top priority. Predicting the number of bikes needed to maintain a steady supply of rental bikes at each hour's interval is essential.With the help of these bike sharing programmes, users can hire a bike from one spot and return it to another or the same location as needed. Bikes can be rented by members or on a need-basis.
On the basis of previous usage patterns in connection to weather, time, and other data, we were tasked to anticipate the demand for bike sharing. Provided with the Bike Sharing dataset, it contained weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

## Project Execution
We followed the following steps to achieve our objective for the project:

* Understanding the dataset, performing some basic data inspection to verify the number of columns, comprehending data distribution, and examining the statistics for each variable.
* Performing Exploratory Data Analysis to get maximum insights from the raw dataset as well as visualising the data to make these insights easily undertandable to stakeholders. This included various Univariate, Bivariate and Multivariate analysis.
* Data processing that includes taking care of missing values, outlier detection using box-plots and outlier removal using IQR and technique, multicolliniearity detection using collinearity heatmap and handling multicollinearity by calculating VIF for each feature.
* Feature Engineering, which is creating new features, dropping the unnecessary ones, converting categprical features into numerical using Label encoding and getting new features from a multi-label categorical feature using One Hot Encoding and finally Feature Selection before model building.
* Defining model prerequisits such as Train-Test split, Feature transformation, Feature Scaling and setting hyperparameters.
* Experimenting with various ML algorithms and getting their evaluation scores and feature importances.
* We experimented using simple Linear Regression model, Decision Trees, Random Forest, XGBoost, Gradient
Boosting Machine, LightGBM and CatBoost model. We employed Hyperparameter Tuning using GridsearchCV on the tree based models.
* We finally concluded the project with XGBoost giving the best model performance followed by LightGBM and Gradient
Boosting Machine.

# Project Conclusion and Inference
We observed the following conclusions after executiong this project:

* There is not much of a linear relation between the features and the target in
the given dataset, so we have to move beyond the scope of linear regression
to achieve more accurate results and better model performance
* Temperature is the most prominent feature as derived from Decision Trees,
Random Forest, Gradient Boosting Machine, LightGBM, CatBoost.
* Functioning Day is the most prominent feature as derived from Linear
Regression and XGBoost models.
* XGBoost seems to be performing better as compared to other models.
However, it is the only feature along with linear regression that suggests
Functioning Day to be the most important feature
* Gradient Boosting Machine and CatBoost give a pretty similar performance
with Temperature being their most important feature.

* Model Performance: 
1. XGBoost: 0.797
2. CatBoost: 0.793
3. Gradient Boosting Machine: 0.791
4. LightGBM: 0.789
5. Random Forest : 0.724
6. Decision Trees: 0.692
7. Linear Regression: 0.529

### Overall model performance achieved: 80%
