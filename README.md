# Codes and Papers that I read
Here I upload the paper I ready to replicate and codes I wrote.
### ipynb file
1.Mutual Information_KNN_Forward Search.ipynb
It's the initial code that I used for optimal lag selection.In the code,the dataset I use is Dow Jones Index from 2002-06-13 to 2022-06-13. I mainly use the mutual information based on knn algorithm as information score and forward selection to generate a feature subset. But I failed.

2.Time Series.ipynb
I check the stationarity of dow jones stock time series using ADF test and find the time series after being differenced once is stationary. SO I plot the ACF and PACF for each column(feature) and use 3 Information Criterions: AIC,BIC,HQIC to determine the optimal lag for each feature.

3.All Feature Selection Method.ipynb
There are 3 types of datasets: original,differenced_once and the one after minmax scaling.
I also encapsulate mutual information,maximum information coefficient and partial correlation into functions to generate new feature subsets which include feature names.

The original feature sets is {High(t),Open(t),Low(t),Volume(t)},and the target variable is Close(t+1).
### pdf file: reference papers't titles here 

The picture below is the flow chart that represents the framework of my dissertation
![Pipeline_Optimal_Lag](https://user-images.githubusercontent.com/47016879/176543198-6128b9e5-e270-4768-9fad-4a06af1fce4f.png)
And Now I'm stll working on finding more metrics that can measure the dependency and relationship between the features and the target.

Next,I am gonna use ace as another metric and also search for other multivariate time series.
