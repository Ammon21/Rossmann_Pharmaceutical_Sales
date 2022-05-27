# Rossmann_Pharmaceutical_Sales
# Rossmann Pharmacueticals Sales Forecast


**Table of content**

  - [Overview](#overview)
  - [Objective](#Objective)
  - [Requirements](#requirements)
  - [Install](#install)
  - [Data](#data)
  - [Features](#features)
    - [Data Processing and Analysis](#data-processing-and-analysis)
    - [Scripts](#scripts)
    - [Test](#test)

## Overview

Rossmann Pharmaceuticals are multi-citiy pharmaceuticals stores. The company's finance team is 
in need of sale forecast in all of their stores across several cities six weeks ahead of time
managers in individual stores rely on their years of experience as well as their personal judgement
to forecast sales until now.

## Objective

to build and serve an end-to-end product that delivers this prediction to analysts in the finance team.

## Requirements
  Python 3.7 and above, mlflow, logging, dvc, sklearn, matplotlib, seaborn.


## Install
```
git clone https://github.com/Ammon21/Rossmann_Pharmaceutical_Sales
cd Rossmann_Pharmaceutical_Sales
pip install -r requirements.txt
```

## Data and Features

The data for this challenge can be found [here, Rossmann Store Sales | Kaggle](https://www.kaggle.com/competitions/rossmann-store-sales/data)

### Data fields
 
- Store - a unique Id for each store
- Sales - the turnover for any given day (this is what you are predicting)
- Customers - the number of customers on a given day
- Open - an indicator for whether the store was open: 0 = closed, 1 = open
- StateHoliday - indicates a state holiday. Normally all stores, with few exceptions, are closed on state   holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None
- SchoolHoliday - indicates if the (Store, Date) was affected by the closure of public schools
- StoreType - differentiates between 4 different store models: a, b, c, d
- Assortment - describes an assortment level: a = basic, b = extra, c = extended. Read more about assortment here
- CompetitionDistance - distance in meters to the nearest competitor store
- CompetitionOpenSince[Month/Year] - gives the approximate year and month of the time the nearest competitor was opened
- Promo - indicates whether a store is running a promo on that day
- Promo2 - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating
- Promo2Since[Year/Week] - describes the year and calendar week when the store started participating in Promo2
- PromoInterval - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

## Features
the folder structure
![structure](outputs/folder_structure.txt)

### Data Processing and Analysis
  - ![ML pipeline design](plots/mlpipe.jpg?raw=true)
  
### Scripts
 - All the scripts used by the notebooks are inside the scripts folder.

### Test
 - Tests for the scripts are inside the tests folde