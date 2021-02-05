# Boston_AirBnB

This is the analysis for **Boston AirBnB** data. These analysis answer three business/real world questions.

Question 1--> What are the factors of price variability?
Question 2--> Is there any correlation between the availability of rents and the price?
Question 3--> Can the company impact the monthly variation of rents after analyzing the year long trend?

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting_started)
	1. [Dependencies](#dependencies)
	2. [Cloning](#cloning)
	3. [Executing Program](#execution)
3. [Author](#authors)
4. [License](#license)

<a name="descripton"></a>
## Description

This project aims to develop a stock price prediction machine learning model and then deploy. There are three stages for this project

1. First create a machine learning model for the time series data extracted from Yahoo Finance
2. Develop a local web app using python's Flask library 
3. Deploy the final app in Heroku cloud platform to run the application on the cloud
<a name="getting_started"></a>

<a name="getting_started"></a>
## Getting Started

<a name="dependencies"></a>
### Dependencies
* Python 3.6+
* Visualization libraries: Matplotlib
* Libraries for data and array: pandas and numpy
* Machine learning libraries:Tensorflow, Keras, Scikit-Learn
* Web App library: Flask
* Financial data parsing library: Yfinance 

<a name="cloning"></a>
### Cloning
To clone the git repository:
```
git clone https://github.com/mdsohelmahmood/stock-price-predict
```

<a name="execution"></a>
### Executing Program:
### Part 1

First step is to craete an ML model for the time series data from historical stock price. Data extracted from Yahoo Finance using YFiance library.

#### stock = yf.Ticker("BTC-USD")

The model is created with 30 days prediction input data to predict the days ahead. The will be user flexibility to define this number. This number will 
point on how many days ahead in the future, the user wants to predict. The model is built with 3 layers of LSTM and dropout features to minimize the overfitting.

### Part 2

Next step is to deploy the app in the local server using Flask and predict the stock price. For this, a seperate virtual environent is created and the app is 
deployed in localhost. Two html files are used to take the user input and show the predicted output.


### Part 3

The final step is to deploy it on Heroku cloud platform for everybody to get access and use. The free account in Heroku provides 500 Mb of RAM which is not enough 
for training the model using tensorflow on the fly. Tensorflow itself consumes 300+ Mb. Therefore later, I built and saved the model. Since the model has all the necessary information to predict the test data and no tensorflow is rquired, it is less than 500 Mb limit and can be easily deployed in Heroku.



<a name="authors"></a>
## Author

* [Md Sohel Mahmood](https://github.com/mdsohelmahmood)

<a name="license"></a>
## License
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Screenshots
![Web App](https://github.com/mdsohelmahmood/stock-price-predict/blob/main/Latex/Figures/form.png)
![Web App](https://github.com/mdsohelmahmood/stock-price-predict/blob/main/Latex/Figures/plot.png)


