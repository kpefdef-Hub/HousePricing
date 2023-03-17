# HousePricing
Using SAS, I permformed an analysis with multiple regression model on a dataset containing several factors including the prices of homes to identify the factors that influence the prices. Then I used the model to estimate the prices of houses coming on the market.


![house price](https://user-images.githubusercontent.com/114897374/225780129-f79a8a23-7a74-4f42-b200-0303b0ff6534.png)


Explaining the Coefficient
●	The intercept coefficient (-120921) represents the estimated price of the House when the input values are at zero
●	The BsmtSF coefficient (19.8187) represents the expected increase in the price of the House for every 1-unit increase in the square footage of the basement, with all other input values remaining constant
●	The bsmtFullBath coefficient (13428.4) represents the expected increase in the price of the House for every 1-unit increase in the number of full bathrooms in the basement, with all other input values remaining constant
●	The condition  (3033.0) represents the expected increase in the price of the House for every 1-unit increase in the condition of the house, with all other input values remaining constant
●	The firePlaces coefficient (4869.4) represents the expected increase in the price of the House for every 1-unit increase in the number of fireplaces, with all other input values remaining constant
●	The floorOneSF coefficient (47.2156) represents the expected increase in the price of the House  for every 1-unit increase in the square footage of the first floor, with all other input values remaining constant
●	The floorTwoSF coefficient (41.0270) represents the expected increase in the price of the House  for every one-unit increase in the square footage of the second floor, with all other input values remaining constant
●	The coefficient for garageCars (1.7243.4) represents the expected increase in the price of the House for every one-unit increase in the number of cars that can fit in the garage,  with all other input values remaining constant
●	The lotArea coefficient (0.4019) represents the expected increase in the price of the House for every one-unit increase in the square footage of the lot area, with all other input values remaining constant
●	The noRooms coefficient (430.4) represents the expected increase in the price of the House for every one-unit increase in the number of rooms above ground, with all other input values remaining constant. The p-value for this coefficient (0.6904) is not significant since it is greater than the confidence level 0.05, which means that this input value does not have an effect on the price of the house
●	The quality coefficient (23831.7) represents the expected increase in the price of the House for every one-unit increase in the quality rating of the house, with all other input values remaining constant
●	The woodDeckSF coefficient (34.8805) represents the expected increase in the price of the House for every one-unit increase in the square footage of the wood deck, with all other input values remaining constant

Explaining the Model
The following inputs influence the price of the house:
●	square footage of the basement - 0.0001
●	the number of full bathrooms in the basement - 0.0001
●	condition of the house - 0.0008
●	the number of fireplaces - 0.0069
●	the square footage of the first floor - 0.0001
●	the square footage of the second floor - 0.0001
●	the number of cars that can fit in the garage - 0.0001
●	the square footage of the lot area - 0.0002
●	the quality rating of the house - 0.0001
●	the square footage of the wood deck - 0.0001 

The following input however do not influence the price of the house:
●	the number of rooms above ground - 0.6904
The p-value of the model at 0.0001 is statistically significant and tells us we can trust the results of the model.


Explaining the R-Square 
A value of 0.7813 for R-squared indicates that approximately 78.13% of the variation in the dependent variable is explained by the independent variable(s) in the model. 
This means that factors in the regression model influences 78.13% of the price of the house. The remaining 21.87% may be influenced by the other properties satisfaction that are not included in the analysis.

Mathematical equation for the model
=     -120921 + (19.8187 * BsmtSF) + (13428.4 * bsmtFullBath) + (3033.0 * condition) + (4869.4 * firePlaces) + (47.2156 * floorOneSF) + (41.0270 * floorTwoSF) + (1.7243.4 * garageCars) + (0.4019 * lotArea) + (430.4 * noRooms) + (23831.7 * quality) + (34.8805 * woodDeckSF)


Estimated Prices

![Screenshot (63)](https://user-images.githubusercontent.com/114897374/225780712-f9ea67e0-f0b8-4b9c-a370-86fda9416369.png) 



