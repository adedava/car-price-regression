# Car Price Regression
This project aims to predict car prices using deep learning techniques. The models focus on comparing simple and complex neural network architectures, with an emphasis on understanding how model complexity affects performance on a small dataset.

## Dataset
The dataset contains various car attributes used to predict price.

Key features include:
* Engine size  
* Horsepower  
* Fuel type  
* Car dimensions  
* Mileage (city-mpg, highway-mpg)  

## Data Preprocessing
Several preprocessing steps were applied:

* Handling missing values  
* Converting data types from object to numeric  
* Separating numerical and categorical features  
* Encoding categorical variables using one-hot encoding  
* Scaling numerical features  
* Applying logarithmic transformation on the target variable  

## Models
Three neural network models were implemented:

* Model 1 (Simple Architecture)  
* Model 2 (Deeper Architecture)  
* Model 3 (Complex Architecture with Dropout)  

## Results
| Model   | MAE      | RMSE     |
|--------|----------|----------|
| Model 1 | ~11,500 | ~15,700 |
| Model 2 | ~11,600 | ~15,900 |
| Model 3 | ~30,000 | ~89,000 |

Model 1 and Model 2 produced similar performance, while Model 3 performed significantly worse.

## Key Insights
* Increasing model complexity does not necessarily improve performance  
* Complex models tend to perform poorly on small datasets  
* Simpler models provide more stable and consistent predictions  
* Dropout and deeper architectures can lead to underfitting when data is limited  
* Deep learning is not always optimal for tabular datasets  

## Conclusion
Simpler neural network architectures perform better than more complex models for small tabular datasets. Model complexity should be adjusted based on data size and characteristics.
