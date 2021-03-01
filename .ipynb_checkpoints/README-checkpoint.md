![Crypto Sneaks Logo](images/CryptoSneaks.gif)

## Table of Contents

* [Summary](#summary)
* [Resources](#resources)
* [Exploratory Data Analysis](#exploratory-data-analysis) 
* [Modeling](#modeling)
---
## Summary

---
## Data Source 
![Stockx_image](images/stockxlogo.png)

StockX provided data in 2019 as part of its [StockX Data Contest](https://stockx.com/news/the-2019-data-contest/), te dataset consist of 99,956 transactions from 2017 to 2019, two brands, and over 50 different styles. 

![data_source](MarketAnalysis/media/data_source.png)

---
## Exploratory Data Analysis
Using the dataset provide by StockX we evaluated the different aspects 
[Sneakers Analysis](MarketAnalysis/notebooks/Sneakers_Data_Analysis.ipynb)

![by_name](MarketAnalysis/media/by_name.png)


![by_retail_price](MarketAnalysis/media/by_retail_price.png)


![by_shoe_size](MarketAnalysis/media/by_shoe_size.png)


![by_region](MarketAnalysis/media/by_region.png)


![avg_sale_price](MarketAnalysis/media/avg_sale_price.png)

---
## Modeling
[Random Forest Regression](MarketAnalysis/notebooks/Random_Forest_Regression.ipynb)

### Parameters
```python
# Define features set
X = df.drop(['sale_price'], axis=1)

# Define target vector
y = df.sale_price

# Encoding variables
X = pd.get_dummies(X, columns=["brand", "sneaker_name", "buyer_region"])
X.head()

# Splitting into Train and Test sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state = 27)

# Create the random forest regresor instance
rf_model = RandomForestRegressor(n_estimators=500,random_state=27)
```

### Results
![feature_importances](MarketAnalysis/media/feature_importance.png)

### Metrics
```python
R²: 0.98
Mean Absolute Error: 14.49
Median Absolute Error: 7.10
Accuracy: 97.14%
```