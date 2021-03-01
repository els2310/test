![Crypto Sneaks Logo](images/CryptoSneaks.gif)

## Table of Contents

* [Summary](#summary)
* [Resources](#resources)
* [Exploratory Data Analysis](#exploratory-data-analysis)
  * [Analysis by Sneakers Name](#analysis_by_sneakers_name)
  * [Analysis by Retail Price](#analysis_by_retail_price)
  * [Analysis by Shoe Size](#analysis_by_shoe_size)
  * [Analysis by Region](#analysis_by_region)
  * [Analysis by Ordered Date](#analysis_by_ordered_date)
  * [Analysis by Average Resale Price](#analysis_by_average_sales_price)  
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

### Analysis by Sneaker Name
![by_name](MarketAnalysis/media/by_name.png)

### Analysis by Retail Price
![by_retail_price](MarketAnalysis/media/by_retail_price.png)

### Analysis by Shoe Size
![by_shoe_size](MarketAnalysis/media/by_shoe_size.png)

### Analysis by Region
![by_region](MarketAnalysis/media/by_region.png)

### Analysis by Average Resale Price
![avg_sale_price](MarketAnalysis/media/avg_sale_price.png)

---
## Modeling
[Random Forest Regression](MarketAnalysis/notebooks/Random_Forest_Regression.ipynb)

### Parameters
![rf_one](MarketAnalysis/media/rf_model_one.png)
![rf_two](MarketAnalysis/media/rf_model_two.png)

### Results
![predict-actual](MarketAnalysis/media/predict-actual.png)
![feature_importances](MarketAnalysis/media/feature_importances.png)
![metrics](MarketAnalysis/media/metrics.png)
