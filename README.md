# Tehran House Price Regression

machine learning project for predicting apartment prices in Tehran using regression models.

## Project overview

This project uses a real housing dataset with about 3,500 apartment records. The notebook follows workflow: understand the data, clean incorrect values, explore important patterns, prepare the features, train regression models, and compare their performance.

The main prediction target is Price in Toman.

## Dataset information

The dataset contains these columns:

- `Area` - apartment area in square meters
- `Room` - number of rooms
- `Parking` - parking availability
- `Warehouse` - storage room availability
- `Elevator` - elevator availability
- `Address` - approximate Tehran neighborhood/area
- `Price` - price in Toman
- `Price(USD)` - price in US dollars

The raw data includes missing addresses and a few incorrect very large `Area` values. The notebook removes these rows during cleaning.

Dataset source provided with the course/project:  
https://maktabkhooneh.org/lms/course/%DB%8C%D8%A7%D8%AF%DA%AF%DB%8C%D8%B1%DB%8C-%D9%85%D8%A7%D8%B4%DB%8C%D9%86-%D9%BE%D8%A7%DB%8C%D8%AA%D9%88%D9%86-mk1318/unit/42338/
www.kaggle.com/mokar2001/house-price-tehran-iran

## Features used

The models use:

- Area
- Room
- Parking
- Warehouse
- Elevator
- Address (one-hot encoded)

`Price(USD)` is not used as an input because it is a converted version of the same target price and would cause target leakage.

## Machine learning methods used

- Simple Linear Regression
- Polynomial Regression (degree 2)
- Multiple Linear Regression
- Train/test split
- One-hot encoding for `Address`
- MAE, RMSE, and R² for evaluation

## Libraries used

- pandas
- numpy
- matplotlib
- scikit-learn

