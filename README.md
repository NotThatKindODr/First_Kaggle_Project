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

### Which city has the lowest seasonal variance of avocados?

### How do the size/type of avocado factor into the lowest average cost?

### Which city is the lowest average cost when controlling for size and type


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
['West' 'Midsouth' 'Northeast' 'Northern New England' 'South Central' 'Southeast' 'Great Lakes' 'Plains']
```

**Select States**
* West Tex/New Mexico
* California
* South Carolina

```
['California' 'West Tex/New Mexico' 'South Carolina']
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
['Albany' 'Atlanta' 'Baltimore/Washington' 'Boise' 'Boston'
 'Buffalo/Rochester' 'Charlotte' 'Chicago'
 'Cincinnati/Dayton' 'Columbus' 'Dallas/Ft. Worth' 'Denver' 'Detroit'
 'Grand Rapids' 'Harrisburg/Scranton' 'Hartford/Springfield'
 'Houston' 'Indianapolis' 'Jacksonville' 'Las Vegas' 'Los Angeles'
 'Louisville' 'Miami/Ft. Lauderdale' 'Nashville'
 'New Orleans/Mobile' 'New York'
 'Orlando' 'Philadelphia' 'Phoenix/Tucson' 'Pittsburgh'
 'Portland' 'Raleigh/Greensboro' 'Richmond/Norfolk' 'Roanoke' 'Sacramento'
 'San Diego' 'San Francisco' 'Seattle' 'Spokane' 'St. Louis' 'Syracuse' 'Tampa']
 ```