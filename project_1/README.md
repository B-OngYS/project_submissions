# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Exploring climate data of Singapore

### Overview

<font size = "3">Internationally, $CO_2$ emissions has been linked to the increased occurrences of extreme weather events$^1$. Singapore has had extreme weather experiences including the 1997 'haze'$^2$, the 2011 'ponding' of Liat Towers$^3$, and in 2022 flash floods closing sections of the Ulu Pandan park connector$^4$.</font>

<font size='3'>According to the National Climate Change Secretariat (NCCS), a strategy group of the Singapore Prime Minister's office, "[r]ainfall has become more intense in recent years. Annual rainfall total for Singapore has increased at an average rate of 67 mm per decade from 1980 to 2019."$^5$</font>

<font size='3'>$CO_2$ emissions have been rising globally. From data from the world bank, $CO_2$ emissions have risen from 20,625,000 kilotonnes in 1990 to 34,344,006 kilotonnes in 2019. $^6$</font>

<font size='3'>Similarly, Singapore has also increased its $CO_2$ emissions from 28,970 kilotonnes in 1990 to a peak of 49,140 kilotonnes in 2017.$^7$</font>


$^1$ _CO2 Can Directly Impact Extreme Weather, Research Suggests_ (https://www.scientificamerican.com/article/co2-can-directly-impact-extreme-weather-research-suggests/#:~:text=Even%20though%20average%20global%20temperatures,certain%20regions%20around%20the%20world.)

$^2$ _Singapore haze hits record high from Indonesia fires_ (https://www.bbc.com/news/world-asia-22998592)

$^3$ _Overflowing Stamford Canal cause of recent Orchard Rd flash floods: PUB_ (https://sg.news.yahoo.com/heavy-rain-caused-flash-floods-on-23-dec--pub.html)

$^4$ _Sections of Ulu Pandan Park Connector briefly closed after flash flood warning_ (https://www.straitstimes.com/singapore/ulu-pandan-park-connector-section-closed-after-flash-flood-warning)

$^5$ _Impact Of Climate Change In Singapore_ (https://www.nccs.gov.sg/singapores-climate-action/impact-of-climate-change-in-singapore/)

$^6$ _CO2 emissions (kt)_ (https://data.worldbank.org/indicator/EN.ATM.CO2E.KT?contextual=default&end=2019&name_desc=false&start=1990&view=chart)

$^7$_CO2 emissions (kt) - Singapore_ (https://data.worldbank.org/indicator/EN.ATM.CO2E.KT?contextual=default&end=2019&locations=SG&name_desc=false&start=1990&view=chart)
### Problem Statement

<font size = "3">The NEA communications arm has decided to attribute Singapore's extreme weather events to $CO_2$ emissions and has hired me from fiverr.com to recommend the data and visualizations to show how increasing $CO_2$ emissions is changing Singapore's weather.</font>

---

### Datasets

#### Provided Data

There are 8 datasets included in the [`data`](./data/) folder for this project. These correponds to rainfall information. 

* [`rainfall-monthly-number-of-rain-days.csv`](./data/rainfall-monthly-number-of-rain-days.csv): Monthly number of rain days from 1982 to 2022. A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more.
* [`rainfall-monthly-total.csv`](./data/rainfall-monthly-total.csv): Monthly total rain recorded in mm(millimeters) from 1982 to 2022
* [Relative Humidity](https://data.gov.sg/dataset/relative-humidity-monthly-mean)
* [Monthly Maximum Daily Rainfall](https://data.gov.sg/dataset/rainfall-monthly-maximum-daily-total)
* [Hourly wet bulb temperature](https://data.gov.sg/dataset/wet-bulb-temperature-hourly)
* [Monthly mean sunshine hours](https://data.gov.sg/dataset/sunshine-duration-monthly-mean-daily-duration)
* [Surface Air Temperature](https://data.gov.sg/dataset/surface-air-temperature-mean-daily-minimum)
* $CO_2$ emissions data from the World Bank
---

#### Data Dictionary
|Feature|Type|Dataset|Description|
|:-|:-:|:--|:--|
|total_rainfall|*float*|rainfall-monthly-total|Total rainfall in mm|
maximum_rainfall_in_a_day|*float*|rainfall-monthly-highest-daily-total|Highest amount of rainfall in a day for each month in mm|
no_of_rainy_days|*integer*|rainfall-monthly-number-of-rain-days|Number of rainy days each month (A day is considered to have “rained” if the total rainfall for that day is 0.2mm or more)|
mean_rh|*float*|relative-humidity-monthly-mean|The average relative humidity per month (out of 100)|
mean_sunshine_hrs|*float*|sunshine-duration-monthly-mean-daily-duration|The average amount of sunshine per month in hours| 
mean_temp|*float*|surface-air-temperature-monthly-mean|The average surface air temperature per month in degrees Celsius|
wet_bulb_temperature|*float*|wet-bulb-temperature-hourly|The average wet bulb temperature per month in degrees Celsius|
sg_emissions(kt)|*float*|co2_data|The yearly $CO_2$ emissions by Singapore in kilotonnes|
wrld_emissions(kt)|*float*|co2_data|The yearly $CO_2$ emissions by the world in kilotonnes|

### Key takeaways

- Singapore's weather is becoming more extreme and it correlates to the increase in $CO_2$ emissions.
- Median temperatures have risen by about 1 degree celcius
- The variation of the the average surface air temperature has increased over the decades.
- The total monthly rainfall swings to the extremes with more frequent dry spells.

### Recommendations

- Using the temperature, total rainfall and maximum rainfall, NEA can convince its stakeholders (the public and other governemnt agencies) that $CO_2$ emissions are linked to more extreme weather.
- According to data from Our World in Data, electricity makes up the majority of Singapore's $CO_2$ emissions so that is where they should focus their efforts convincing people to be more energy efficient.
- The proportion of using oil for energy is decreasing. More efforts can be put into promoting the use of green energy.
