<h2 align="center">Predicting Bike Sharing Demand 
    <h2 align="center">with Supervised Machine Learning, by Linear Regression (Regression)
</h2>

__1) The Goal:__ Build and train a regression model on the Capital Bike Share (Washington, D.C.) Kaggle data set to predict the total count of bikes rented during each hour covered by the test set, using only the information (time- and weather-related features) available prior to the rental period.   

A practical application of such a project would help you answer the following question, as an example: “Given the forecasted weather conditions, how many bicycles can we expect to be rented out (city-wide) this Saturday at 2pm?”

__2) Get the Data:__ You are provided hourly rental data spanning two years. Download the [Capital Bike Share Dataset](https://www.kaggle.com/c/bike-sharing-demand/data) from Kaggle and explore the data in pandas.   

__3) Split the Data:__ Already split: "train.csv" and "test.csv". The training set is comprised of the first 19 days of each month, while the test set is the 20th to the end of the month. 

__4) Exploratory Data Analysis (EDA)__

__5)-9) Feature Engineering (FE), Train Model, Optimize Hyperparameters/Cross-Validation:__ Optimize the model iteratively, select features, try different regressors (e.g. Linear Regression, Random Forest Regressor, SVR)

__10) Calculate Test Score:__ Because this is a regression problem, we are not evaluating our models using accuracy! Submissions are evaluated on the Root Mean Squared Logarithmic Error RMSLE. The RMSLE is calculated as

<img src="https://render.githubusercontent.com/render/math?math=sqrt{\frac{1}{n} \sum_{i=1}^n (\log(p_i + 1) - \log(a_i+1))^2 }">
sqrt{\frac{1}{n} \sum_{i=1}^n (\log(p_i + 1) - \log(a_i+1))^2 }
Benchmarks:
- RMSLE < 0.5, is excellent! ⭐⭐⭐ 
- RMSLE < 0.75 is also quite solid ⭐⭐ 
- RMSLE > 1.0 means that there is still some FE work to do.  

__11) Deploy and Monitor:__ Submit your prediction to Kaggle.  
