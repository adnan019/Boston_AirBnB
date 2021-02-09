# Boston AirBnB Data Exploratory Analysis

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting_started)
	1. [Dependencies](#dependencies)
	2. [Cloning](#cloning)
	3. [Statement details](#execution)
3. [Summary of results](#summary)
4. [Author](#authors)
5. [License](#license)
5. [Acknowledgements](#acknowledgements)
6. [Screenshots](#screenshots)
7. [Files](#files)

<a name="introduction"></a>
### Introduction

This is the analysis for **Boston AirBnB** data. The motication of this project is to perform explorartory data analysis on Airbnb listing data and answer three business/real world questions.

Question 1--> What are the factors of price variability?
Question 2--> Is there any correlation between the availability of rents and the price?
Question 3--> Can the company impact the monthly variation of rents after analyzing the year long trend?

### CRISP-DM method
* Business understanding – What does the business need? 
* Data understanding – What data do we have / need? Is it clean? 
* Data preparation – How do we organize the data for modeling? 
* Modeling – What modeling techniques should we apply? 
* Evaluation – Which model best meets the business objectives? 
* Deployment – How do stakeholders access the results?

To implement the CRISP-DM method, we first eed to understand the business. The business is oriented towards customer satistaction and will be greatly interested to optimize the variations of rental price. Regarding data, the listing data provided us the price acroos differnt factors like property-type, policy etc. We will demonstrate couple of those factors in this project. The data will be prepared for visualization. We will use descriptive statistics to find answerss to the questions. We do not need modeling, evaluation and deployment to find solutions for the given questions.

<a name="getting_started"></a>

<a name="getting_started"></a>
## Getting Started

<a name="dependencies"></a>
### Dependencies
* Python 3.7
* Visualization libraries: matplotlib, seaborn
* Libraries for data and array: pandas and numpy

<a name="cloning"></a>
### Cloning
To clone the git repository:
```
git clone https://github.com/mdsohelmahmood/Boston_AirBnB
```

<a name="execution"></a>
### Statement details:

### Question 1--> What are the factors of price variability?

Data is procvided for different listings for the past couple of years. In order to find out the underlying factors of price variability, we need to follow the CRISP-DM method and assess. The business is oriented towards customer satistaction and will be greatly interested to optimize the variations of rental price. The listing data provided us the price acroos differnt factors like property-type, policy etc. We will demonstrate couple of those factors in this project.

So, to answer our first question, we need to deep dive on the price variability for different factors such as property type, policy and other accommodations. We found that these prime factors are considerably influencing the variation of rentals. Since the apartment type is widely available, variation in price is also expected. Next the policy was investigated and it came out that the rental with the most strict policy, usually have the highest rent. Finally the bed type plays a pivotal role of the price estimation of the rental. Those having real bed are listed with higher prices compared to other bed types including sofa, futon or couch. 

### Question 2--> Is there any correlation between the availability of rents and the price?

Next we move forward to answer the second question. To find out the relation between availability of rentals and price, we needed to crunch the data with timestamps. We analyzed the data from August 2016 to August 2017 and tried to dig out that relationship. Some interesting incidents were observed when the availability and prices are shown together. Roughly towards the end of 2016 and in February 2017, there were two sharp drops in rental price when in fact the availability did not vary drastically. The trend seemed to stay flat for the rest of the year except a deep dive at some point in April 2017. The price actually mirrored the availability at that time which tells the fundamental rule of demand and supply. The cyclic trend of rental availability is mainly attributed to the fact that weekends offer less number of properties available or listed on the site.. 


### Question 3--> Can the company impact the monthly variation of rents after analyzing the year long trend?

Lastly the monthly variation of rentals are studied to obtain the trend over a year. This is specially crucial for company revenue to be focused on certain months rather than highly depending on peak seasons. Data shows that September and October have the highest rental price (possible off-peak season) due to less availability. The company may interpret this data to dig out the underlying cause and provide to stakeholders.

<a name="summary"></a>
### Summary of results

The observation on the niche parts of Boston Airbnb data divulges the variation of price mainly over property type, bed type and policy. Although the apartments are the most common rentals, high-end apartments are good contenders with villas or full house in terms of price. Other than that, apartments are the most widely listed rentals. Some interesting factor was observed when timestamp data was explored. Some high rises and deep dives are not uncommon for a whole year data. End of the summer season signifies the highest price of the rentals during the year

<a name="authors"></a>
### Author

* [Md Sohel Mahmood](https://github.com/mdsohelmahmood)

<a name="license"></a>
### License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<a name="acknowledgements"></a>
### Acknowledments

* Kaggle as data source (https://www.kaggle.com/airbnb/boston)
* Udacity for providing the opportunity to participate in blog writing

### Screenshots
![Web App](https://github.com/mdsohelmahmood/Boston_AirBnB/blob/main/Figures/3.png)
![Web App](https://github.com/mdsohelmahmood/Boston_AirBnB/blob/main/Figures/price%20and%20availability%20trend%20over%20time.png)

## Files

1. Data_Analysis_Boston_AirBnB.ipynb --> the jupyter notebook file performing the analysis
2. Figures folder --> contains all the figures used on the blog writing
3. A licence file and 
4. A readme.md file


