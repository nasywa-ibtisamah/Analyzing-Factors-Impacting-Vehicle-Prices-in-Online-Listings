# Project Description

Hello there :wave:
I hope this project finds you well!

In this project, I will analyze the factors that influence the price of a vehicle in the listings of vehicle advertisements on the website.

**Objective**
1. Analyze the ad duration
2. Analyze the number of ads and the average price for each type of vehicle.
3. Analyze what factors that most influence the price of a vehicle.


# Steps

1. Data Overview
2. Data Preprocessing
3. Data Analysis

## 1. Exploratory Data Analysis

**Data Description** 
- `price`: vehicle price
- `model_year`: release year of the vehicle
- `model`: vehicle model
- `condition`: vehicle condition
- `cylinders`: the number of cylinders in car's engine
- `fuel` — the fuel of the vehicle
- `odometer` — The distance traveled by the vehicle at the time the advertisement is displayed.
- `transmission`: type of transmission of the car
- `paint_color`: car's paint color
- `is_4wd` — Does the vehicle have four-wheel drive (Boolean type)?
- `date_posted` — The date the advertisement was displayed.
- `days_listed` — The number of days the advertisement was displayed until it was deleted.

## 2. Pre-Processing Data

The following are data preprocessing steps I did in this project:
1. Analyzing patterns of missing values
2. Filling in missing values
4. Fixing incorrect data types
4. Analyzing outliers
5. Removing outliers

## 3. Data Analysis:

1.  Analyzing ad duration
	Findings:
	- The average days_listed or ad duration for all types of vehicles is almost the same, ranging from 38 to 43 days.
	- Some ads are removed quickly within 0 days. This could happen when the car is sold on the same day the ad was posted. The vehicle types with the fastest ad removal time of 0 days are mini-van, van, convertible, pickup, SUV, coupe, truck, hatchback, and sedan.
	- The longest ad duration is 271 days, observed for sedan type vehicles.
	
2. Average Price for Each Vehicle Type
	Findings:
	- The most advertised vehicle types are SUV and sedan.
	- The highest average price is found in the Bus vehicle type.
	- However, the number of ads does not have an impact on the price, as the average price for Sedan is 6965, the average price for SUV is 11149, and the average price for Truck is 16734.

3. Most influential factor on the vehicle's price

	Findings:
	Price is influenced by model_year (corr value is 0.41) , car_age (corr value is -0.41, odometer (corr value is 0.15 and value_condition (corr value is 0.22)




# General Conclusion

**for Data Processing, I did these steps:**

1. Handled Missing Values
2. Fixed incorrect data types
3. Added new column
4. Found out the relation between variable using Correlation Matrix
5. Checked outliers and Removed it
6. Defined Lower Bound and Upper Bound
7. Analyzed the diagram for Dataset with Outliers and Without Outliers

 **Correlations between numeric variables:**

There are correlations between the following variables:
a. Model Year and Price > positively correlated

b. Model Year and Odometer > negatively correlated

c. Price and Odometer > negatively correlated

d. Cylinders and is_4wd > positively correlated

e. is_4wd and Price > positively correlated

f. Value_condition and Price > positively correlated

g. Value_condition and Model_year > positively correlated

**Relationship between price and categorical variables:**

1. The highest price is for cars with the brand Nissan.
2. The highest price is for cars with pickup type.
3. The highest price is for cars with automatic transmission.
4. The highest price is for cars with the color blue.
