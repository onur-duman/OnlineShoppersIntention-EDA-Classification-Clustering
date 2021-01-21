![Build Status](https://api.travis-ci.com/desxz/OnlineShoppersIntention-EDA-Classification-Clustering.svg?branch=main&status=passed)     [![Contributors](https://img.shields.io/badge/Contributors-3-green.svg?style=flat-square)](#contributors-)

# OnlineShoppersIntention-EDA-Classification-Clustering
This repository includes our 2020-2021 Fall Semester Data Mining(CENG3521) Class Final Project. We've used Python language to code and Jupyter Notebook for IDE. And Numpy, Pandas, Matplotlib, Seaborn and Sklearn are libraries which are used for it.

## Team Members(sorted by name)



<table>
  <tr>
    <td align="center"><a href="https://github.com/ahmtgrbz"><img src="https://avatars0.githubusercontent.com/u/44843548?s=460&v=4" width="100px;" alt=""/><br /><sub><b>Ahmet GÜRBÜZ</b></sub></a><br /><br /><sub><b>P. Component Analysis(PCA)</b></sub></a><br /><sub><b>Clustering(K-Means)</b></sub></a></td>
    <td align="center"><a href="https://github.com/desxz"><img src="https://avatars1.githubusercontent.com/u/63814984?s=460&u=e54733ff64da68c0013cff94fb45ca81272802de&v=4" width="100px;" alt=""/><br /><sub><b>Murat GUN</b></sub></a><br /><br /><sub><b>Classification(SGDClassifier)</b></sub></a><br /><sub><b>Classification(MLPClassifier)</b></sub></a></td>
    <td align="center"><a href="https://github.com/onur-duman"><img src="https://avatars1.githubusercontent.com/u/44534189?s=460&u=74a6216bbebfee1609e631f3ce80ab8241bdfc6a&v=4" width="100px;" alt=""/><br /><sub><b>Onur DUMAN</b></sub></a><br /><br /><sub><b>Explotary Data Analysis(EDA)</b></sub></a><br /><sub><b>Classification(k-NN)</b></sub></a></td>
  </tr>
</table>
   
## Requirements Modules and Its Version

* Python `3.7.4`

* Numpy `1.16.5`
* Pandas `0.25.1`
* Matplotlib `3.1.1`
* Seaborn `0.9.0`
* Sklearn `0.21.3`

# Description of The Online Shoppers Intention Dataset

![1](https://www.further.co.uk/wp-content/uploads/2019/04/onlineshoppers002.jpg)

## Dataset Information:

The dataset consists of feature vectors belonging to 12,330 sessions.
The dataset was formed so that each session would belong to a different user in a 1-year period to avoidany tendency to a specific campaign, special day, user profile, or period.

## Description of The Features

Administrative: This is the number of pages of this type (administrative) that the user visited. <br/>
Administrative_Duration: This is the amount of time spent in this category of pages. <br/>
Informational: This is the number of pages of this type (informational) that the user visited. <br/>
Informational_Duration: This is the amount of time spent in this category of pages. <br/>
ProductRelated: This is the number of pages of this type (product related) that the user visited. <br/>
ProductRelated_Duration: This is the amount of time spent in this category of pages. <br/>
BounceRates: The percentage of visitors who enter the website through that page and exit without triggering any additional tasks. <br/>
ExitRates: The percentage of pageviews on the website that end at that specific page. <br/>
PageValues: The average value of the page averaged over the value of the target page and/or the completion of an eCommerce <br/>
SpecialDay: This value represents the closeness of the browsing date to special days or holidays (eg Mother's Day or Valentine's day) in <br/>
Month: Contains the month the pageview occurred, in string form. <br/>
OperatingSystems: An integer value representing the operating system that the user was on when viewing the page. <br/>
Browser: An integer value representing the browser that the user was using to view the page. <br/>
Region: An integer value representing which region the user is located in. <br/>
TrafficType: An integer value representing what type of traffic the user is categorized into. <br/>
VisitorType: A string representing whether a visitor is New Visitor, Returning Visitor, or Other. <br/>
Weekend: A boolean representing whether the session is on a weekend. <br/>
Revenue: A boolean representing whether or not the user completed the purchase. <br/>

## Dataset Origin:

https://archive.ics.uci.edu/ml/datasets/Online+Shoppers+Purchasing+Intention+Dataset

## Source:

C. Okan Sakar
Department of Computer Engineering, Faculty of
Engineering and Natural Sciences, Bahcesehir University,
34349 Besiktas, Istanbul, Turkey

Yomi Kastro
Inveon Information Technologies Consultancy and Trade,
34335 Istanbul, Turkey

## Relevant Papers

Sakar, C.O., Polat, S.O., Katircioglu, M. et al. Neural Comput & Applic (2018)

# Jupyter Notebook Content

* [Importing Data](#1)
* [First-Looking to Data and Analyzing](#2)
    * [First Looking to Df](#3)
    * [Information](#4)
    * [Information about Numerical Values](#5)
* [EDA and Pre-Processing](#6)
    * [Numerical to Categorical](#7)
    * [Distribution of Categorical Features with Histogram](#8)
    * [Month Setting](#9)
    * [Administrative Settings](#10)
    * [Dropping Some Columns](#11)
    * [Outliers and Removing Them](#12)
    * [Correlation on Categoricals](#13)
    * [Changing Type Of Some Columns to Prepare the Models](#13)
* [Classification](#14)
    * [SGDClassifier](#15)
        * [Creating Model](#21)
        * [Fitting](#22)
        * [Predicting](#23)
        * [Accuracy](#24)
        * [Cross Validation](#25)
    * [MLPClassifier](#16)
        * [Creating Model](#26)
        * [Fitting](#27)
        * [Predicting](#28)
        * [Accuracy](#29)
        * [Cross Validation](#30)
    * [MLPClassifier with Different Hidden Layer Sizes](#31)
    * [k-NN](#20)
        * [Finding Optimum K](#44)
        * [Creating Model with Optimum K](#45)
        * [Fitting](#46)
        * [Prediction](#47)
        * [Accuracy](#48)
        * [Confusion Matrix](#49)
* [Clustering](#17)
    * [PCA](#18)
        * [Creating Model](#32)
        * [Fitting](#33)
        * [Explained Variance Ratios](#34)
        * [Selecting Number of PC Components](#35)
        * [Getting X and Y For Each Components](#36)
        * [Plotting](#36)
    * [K-Means](#19)
        * [Optimum K](#38)
        * [Creating Model](#39)
        * [Fitting](#40)
        * [Plotting K-Means with Optimum K](#41)
        * [Plotting with Cluster Centers](#42)
        * [Plotting with Two Different K](#43)
    
# Accuracy Scores
![Accuray Scores](https://i.hizliresim.com/FLSRMY.png)
# Files Structure

## Jupyter Notebook
* > *OnlineShoppersIntention.ipynb* - Notebook used to clean, classify and cluster the dataset.

## Txt
* > *requirements.txt* - Includes the modules which we used, and its version.

## Dataset
* > *online_shoppers_intention.csv* - Dataset which we used.
* > *online_shoppers_intention_cleaned.csv* - Cleaned data set refer that last status, before classification



