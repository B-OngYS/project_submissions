<img src="http://imgur.com/1ZcRyrc.png" style="float: left; margin: 20px; height: 55px">

# Project 4: West Nile Virus Prediction

---
### Overview

The Disease and Treatment Agency, division of Societal Cures In Epidemiology and New Creative Engineering (DATA-SCIENCE) is tasked with creating an effective plan to deploy pesticides throughout the city of Chicago to combat the recent epidemic of West Nile Virus. The goal is to learn from the mosquito population as data is collected over time while reducing the use of expensive and potentially harmful pesticides. The project will be executed as a group, and the end result will be a model that makes predictions about where to spray pesticides.


---
### Problem Statement

The West Nile Virus (WNV) is a dangerous disease that can cause severe illness and even death in humans. The recent epidemic of WNV in the Windy City has raised concerns about the public health and safety of the citizens. The Department of Public Health has set up a surveillance and control system to collect data over time to learn from the mosquito population.

The objective of this project is to create a model that can predict the presence of WNV in mosquitoes in the city of Chicago. This model will help the city officials to decide where to spray pesticides, which will not only save lives but also reduce the cost of pesticide deployment. The model will be based on the data collected from the surveillance and control system set up by the Department of Public Health. 

---

### Datasets

The project utilizes a dataset from Kaggle, which can be found here: https://www.kaggle.com/c/predict-west-nile-virus/.

The dataset will be used to create a model that predicts where the virus is likely to be present, and the predictions will be used to determine where to spray pesticides.

---
### Data Dictionary
|Feature|Type|Description|
|---|---|---|
|Longitude|Float|Longitude returned from GeoCoder|
|Trap|Object|Id of the trap|
|DewPoint|Int|Average Dew Point|
|Tmin|Int|Min Temp|
|TS|Float|Probability of Thunderstorm in a 9 day window|
|RA|Float|Probability of Rain in a 9 day window|
|dayofyear|Object|Day of the year between 1 and 365|
|Species|Object|Species of mostquito|

---

### Technical Report

The technical report comprises three main components. This includes:
- Part 1: Data Cleaning, EDA, Feature Engineering
- Part 2: Modelling
- Part 3: Cost Benefit Analysis

---

### Conclusion and Recommendations

A summary of the ROC AUC scores of the models is as follows:

|Type|Features|Train Score|Test Score|Kaggle Score|
|---|---|---|---|---|
|Logistic Regression| `Trap`,`DewPoint`,`Tmin`,`TS`,`RA`,`Longitude`,`dayofyear`,`Species`|0.829|0.811|0.714|
|Decision Tree| `Trap`,`DewPoint`,`Tmin`,`TS`,`RA`,`Longitude`,`Species`|0.807|0.789|0.629|

Based on the cost benefit analysis, we see that the benefit-cost ratio option for targeted spraying at the predicted traps is 25.1, while the benefit-cost ratio of mass spraying over chicago is 0.907. A benefit cost ratio of greater than 1 indicates that the program is generating more benefits than costs, and is therefore considered a cost-effective program. This means that for every dollar spent on the vector control program, spraying at the predicted spray areas will see a benefit of $21.20 in reduced healthcare costs. 

Since targeted spraying has a significantly higher benefit to cost ratio than mass spraying,  members of the CDC should consider spraying at the targeted spray sites particularly those with higher probability of WNV present for greater cost efficiency. 

It's worth noting that this calculation only takes into account the direct benefits and costs of the program, and does not include any indirect benefits or costs, such as other side effects of the pesiticides (e.g. individuals with respiratory problems, allergies, or other health conditions may be more vulnerable to the effects of Zenivex).

--- 
