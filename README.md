# Avocado Price Analysis
## What is this data?
Avocado sales from January 4th, 2015 to November 29th, 2020 from that Hass Avocado Board (HAB). The original ask of this data was to find a city where milennials could both afford their avocado toast obsession and to finally move out of their parents' basement.

### Columns 
* date
* average_price - Average price of a single avocado
* total_volume - Number of avocado sold
* 4046 - Number of avocados sold with 4046 PLU (small avocado)
* 4225 - Number of avocados sold with 4225 PLU (large avocado)
* 4770 - Number of avocados sold with 4770 PLU (all avocado, including smaller than small)
* total_bags - total bags of avocado's sold
* small_bags - total small bags
* large_bags - total large bags
* xlarge_bags - total xlarge bag
* type - Coventional or Organic
* year 
* geography - Location, a mixture of total US, region, and city. Need to be careful, see Geography Notes below

## Questions to Answer
### Which city has the lowest average cost of avocados?
Pheonix/Tuscon, Dallas/Ft. Worth, and Houston are by far the cheapest places to buy avocados over the past 5 years. Conversely, Hartford/Springfield, San Franscisco, New York, and Boston are the most expensive.

![plot1](https://github.com/NotThatKindODr/First_Kaggle_Project/blob/main/plots/Location%20and%20Price.png?raw=true)
### Which city has the lowest variance of avocados?
Pittsburgh has the lowest variance in avocado prices at a SD of about $0.20 and an average price of $1.20. San Francisco has the largest variance with about $0.50 over 5 years and being the second most expesnive with an average price of about $1.30. It is possible that cost of living has changed drastically over the past 4 years in California, driving up the price and causing the big swing in varience. I will investigate that question in the second version of the analysis. 

![plot2](https://github.com/NotThatKindODr/First_Kaggle_Project/blob/main/plots/Location%20and%20Varience.png?raw=true)
### How do the size/type of avocado factor into the lowest average cost?


## Next Steps
* Add National Average to Plot1 by using Total U.S. data
* Combine Plot1 and Plot2 by adding the SD as error bars on Plot1
* Look at the price changes over time
* Apply the model of controlling for size and organic v. non-organic

#### Geography Notes
**All of US**
* Total U.S.
```
['Total U.S.']
```

**US Regions**
* West
* Midsouth
* Northeast
* Great Lakes
* Northern New England
* South Central
* Southeast
* Plains

```
['West', 'Midsouth', 'Northeast', 'Northern New England', 'South Central', 'Southeast' 'Great Lakes', 'Plains']
```

**Select States**
* West Tex/New Mexico
* California
* South Carolina

```
['California', 'West Tex/New Mexico', 'South Carolina']
```

**Cities**
* Albany 
* Atlanta
* Baltimore/Washington
* Boise
* Boston 
* Buffalo/Rochester
* Charlotte
* Chicago
* Cincinnati/Dayton
* Columbus
* Dallas/Ft. Worth
* Denver
* Detroit
* Grand Rapids
* Harrisburg/Scranton
* Hartford/Springfield
* Houston
* Indianapolis
* Jacksonville
* Las Vegas
* Los Angeles
* Louisville
* Miami/Ft. Lauderdale
* Nashville
* New Orleans/Mobile
* New York
* Orlando
* Philadelphia
* Phoenix/Tucson
* Pittsburgh
* Portland
* Raleigh/Greensboro
* Richmond/Norfolk
* Roanoke
* Sacramento
* San Diego
* San Francisco 
* Seattle
* Spokane
* St. Louis
* Syracuse
* Tampa
```
['Albany', 'Atlanta', 'Baltimore/Washington', 'Boise', 'Boston',
 'Buffalo/Rochester', 'Charlotte', 'Chicago',
 'Cincinnati/Dayton', 'Columbus', 'Dallas/Ft. Worth', 'Denver', 'Detroit',
 'Grand Rapids', 'Harrisburg/Scranton', 'Hartford/Springfield',
 'Houston', 'Indianapolis', 'Jacksonville', 'Las Vegas', 'Los Angeles',
 'Louisville', 'Miami/Ft. Lauderdale', 'Nashville',
 'New Orleans/Mobile', 'New York',
 'Orlando', 'Philadelphia', 'Phoenix/Tucson', 'Pittsburgh',
 'Portland', 'Raleigh/Greensboro', 'Richmond/Norfolk', 'Roanoke', 'Sacramento',
 'San Diego', 'San Francisco', 'Seattle', 'Spokane', 'St. Louis', 'Syracuse', 'Tampa']
 ```