### Project Overview
#### Title: Maverik Sales Forecasting

#### Introduction
Maverik sales forecasting was the project for my capstone during the MSBA program. This project aims to provide sales forecast for a new Maverik store's first year of sales. There are 4 sales KPIs that need to be forecasted using the numerical and categorical data provided by Maverik for 37 stores' first year of sales. This model needs to be able to capture trend and seasonality in the data and be able to ingest new data and provide forecasts on that, hence, a rolling forecast. This is a time-series forecasting problem. Some models to explore are XGBoost, ARIMA, ETS and Prophet. 

#### Data Exploration and Preprocessing
- There were two datasets. One with historical sales and the other with categorical featuers of stores.
- There are 4 sales target variables, inside sales, food service sales, diesel and unleaded.
- There was one store with unusually high diesel sales, which was removed from training.
- Overall data shows weekly and yearly seasonality with sales being high over the summer months.
- Categorical columns were one-hot encoded.
- New feature was added for the season.
- New data was added to account for any influence of national gas prices.

#### Modeling
- One store was randomly selected as the hold-out store.
- The rest of the stores were used for training.
- After experimenting with XGBoost, ARIMA, ETS and Prophet, the model with the lowest RMSE and MAPE was Prophet.

#### Results
- All RMSEs were significantly below the benchmarks provided by Maverik which was based on a Naive model
- Our model reduced the prediction error by 73% compared to the benchmarks

#### Conclusion
This project was done in collaboration with 3 other MSBA students. We acheived the goal of providing Maverik with sales forecasts for a new Maverik store based on the numerical and categorical data provided. Not only did we produce a model that beat the benchmark significantly, we also won first place in competition with 9 other teams. 

#### Next Steps
If I wanted to expand the scope of the project or ever revisit it, I would experiment with feature selection and optimize the code to increase computational efficiency for the model. 


