# Flight Price prediction Regression

## <b>PROBLEM CONTEXT
<b>

- The goal of this project is to build a predictive regression model that can be useful to forecast the flight fare based on various factors 
- Flight ticket prices are highly unpredictable, often changing day to day, today we might see a price, check out the price of the same flight tomorrow, it will be a different story, making it challenging for travelers and airlines to forecast costs.


## <b>DATASET OVERVIEW

#### <b>Feature	Description

- <b>Airline</b><br>
This column will have all the types of airlines like Indigo, Jet Airways, Air India,  and many more.

- <b>Date_of_Journey</b><br>
This column will let us know about the date on which the passenger's journey will start.

- <b>Source</b><br>
This column holds the name of the place form where the passenger's journey will start.

- <b>Destination</b><br>
This column holds the name of the place to where passengers wanted to travel.

- <b>Route</b><br>
Here we can know about what the route is through which passengers have opted to travel form his/her source to their destination.

- <b>Arrival_Time</b><br>
Arrival time is when the passenger will reach his/her destination.

- <b>Duration</b><br>
Duration is the whole period that a flight will take to complete its journey form source to destination.

- <b>Total_Stops</b><br>
This will let us know in how many places flights will stop there for the flight in the whole journey.

- <b>Additional_Info</b><br>
In this column, we will get information about food, kind of food, and other amenities.

- <b>Price</b><br>
Price of the flight for a complete journey including all the expenses before onboarding.


# <b>TASK 1
### <b>PREPARE A COMPLETE DATA ANALYSIS REPORT ON THE GIVEN DATA.


# <b>TASK 2
### <b>CREATE A PREDICTIVE MODEL WHICH WILL HELP THE CUSTOMERS TO PREDICT FUTURE FLIGHT PRICES AND PLAN THEIR JOURNEY ACCORDINGLY.



### <b>TYPE OF MACHINE LEARNING PROBLEM.
- <b>It is a Regression problem, where given the above set of features, we need to estimate pric.<br>
### <b>LIST OF ALGORITHMS USES FOR Regression
<b>
    
- Linear Regression
- Support Vector Regressor
- DecisionTreeRegressor
- RandomForestRegressor
- GradientBoostingRegressor
- XGBRegressor


# Result
| S.No | Algorithm                | Train R-squared | Test R-squared | Cross Val Score |
| ---- | ------------------------ | --------------- | -------------- | --------------- |
| 1    | Linear Regression        | 0.64            | 0.64           | 0.633269        |
| 2    | SVR                      | 0.01            | 0.01           | 0.006415        |
| 3    | SVR Tuning               | 0.61            | 0.61           | 0.613411        |
| 4    | Decision Tree            | 0.96            | 0.67           | 0.667105        |
| 5    | Decision Tree Tuning     | 0.75            | 0.75           | 0.724305        |
| 6    | Random Forest            | 0.95            | 0.79           | 0.793353        |
| 7    | Random Forest Tuning     | 0.89            | 0.82           | 0.809537        |
| 8    | Gradient Boosting        | 0.76            | 0.75           | 0.748531        |
| 9    | Gradient Boosting Tuning | 0.91            | 0.83           | 0.825861        |
| 10   | XGBoosting               | 0.92            | 0.83           | 0.823278        |
| 11   | XGBoosting Tuning        | 0.90            | 0.84           | 0.828162        |



# Summary
#### <b>Best Overall Model: Tuned XGBoost
- With the highest test R² (0.84) and cross-validation score (0.828), it shows excellent balance between performance and generalization.<br>

#### <b>Top Contenders:<br>
- Tuned Gradient Boosting (Test R²: 0.83)
- Tuned Random Forest (Test R²: 0.82)<br>

#### <b>Models to Avoid:
- Untuned SVR (Very poor fit)
- Untuned Decision Tree (Overfits badly)

#### <b>Tuning Matters:
- Across all models, tuning improves test and CV scores, proving the value of hyperparameter optimization.
