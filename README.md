# Practical-Application-Mod-11
This repository contains the files for module 11 assignment.
Identifying factors that drives pricing and customer sales.

## Description of Files
- 'data.csv' - this file contains the data with all the factors that were captured for car sales. 
- 'car_sales.ipynb' - this file contains the code that identifies the various factors that drive prices and sales.

## Business Understanding
- import, mine, and cleanse data that is currently available under vehicles.csv
- dimensionality reduction and clustering for identifying patterns
- cleaning the data to remove any noise
- idenifty possible trends that may impact price/sales

## Data Understanding
- describe dataset to see all numeric values
- check data structure
- check counts for NaN values across the data set
- check counts of unique values across all fields to see what to keep.

## Data Preparation
- removed 'size' column as it has more than 50% NaN
- removed 'region', 'model', 'state', 'VIN', 'manufacturer' as it has too many non numeric unique values
- format the year from float to int to remove decimal place
- removed the price outliers keeping only those 1M and under
- removed odometer outliers keeping only those 200k and under
- removed year outliers and keeping those that have a large amount of purchase from 1990 on.

## Modeling
### Linear Regression Model
  - linear regression model score at 1
  - drive and transmission appears to have the highest positive coeff. which has a positive corrlation impact on the price.
  -  fuel and title has the strongest negative coorlation out of the factors we are looking at.
  -  score for all three means are practially 0 which is to be expected at regression score at 1
### Polynomial Regression Model
  - highest coorlation is the fuel_gas
  - Polynomial regression model score at 1
  -  score for all three means are practially 0 which is to be expected at regression score at 1

## Evaluation
- appears that both models I ran the data through shows a score of 1. seems unlikely that were to happen.
- but both models show that outside of year (later years), odometer(low miles), make (low to mid brand) - which we expect to impact price and sales, the fuel type of car is the seems to hav a high coorelation with price.
- may want to just look at more indiviual factors as oppose to the ones i have selected, but also keep some noise. i think i narrorwed down the data too much to not take into account any noise. so everything that is tested always falls with score of 1.
- plots shows trending for certain fields that does drive sales and price which leads to customer sales.

## Deployment
- Factors that drive sales and what customers want are what we exoect, but there seems to be a coorlation between at fuel type with diesel driving price high.
- Manufacturs of lower to mid range along with new cars is what is driving sales of cars. 
- trending shows that price of 150k is roughly the cutoff to not have cars sitting on the lot for cars in general but while keeping a few on hand for those who want to spend more.
- to keep inventory at the right level Inventory should be slotted with later year models with the older models not as deserible.



  
