![GitHub Repo stars](https://img.shields.io/github/stars/rppradhan08/ecom-rfm-segmentation)
![GitHub forks](https://img.shields.io/github/forks/rppradhan08/ecom-rfm-segmentation?color=green)
![contributors-shield](https://img.shields.io/github/contributors/rppradhan08/ecom-rfm-segmentation)

<h1 align="center">
  <br>
  <a href="https://github.com/rppradhan08/ecom-rfm-segmentation"><img src="C:\Users\RAJPRAVEEN\Desktop\Projects\E-Commerce Customer Segmentation\images\Customer-segmentation.png" alt="Customer Segmentation" width="200"></a>
  <br>
  Customer Segmentation
  <br>
</h1>

<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About the Project](#about-the-project)
  - [Business Problem](#business-problem)
    - [Task](#task)
  - [Approach](#approach)
    - [Steps Involved](#steps-involved)
- [Getting Started](#getting-started)
  - [Installations](#installations)
  - [Overview and understanding of data](#overview-and-understanding-of-data)
  - [Data preprocessing](#data-preprocessing)
  - [Data Prepeparation](#data-prepeparation)
  - [Cluster assignment using K-means clustering](#cluster-assignment-using-k-means-clustering)
  - [Recommendations](#recommendations)
- [Contacts](#contacts)

# About the Project

In this project, I have used [E-Commerce dataset](https://www.kaggle.com/carrie1/ecommerce-data) from Kaggle to perfrom RFM Analysis and used K-means clustering to segment customers into different clusters based on their behavioural characheristics.

## Business Problem

As a manager of the online store, you would want to group the customers into different clusters, so that you can make a customised marketing campaign for each of the group. You would have to decide what the important business criteria are on which you would want to segregate the customers. This is a transnational data set which contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail.The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

### Task

- Decide the important business criteria to segregate he customers
- Group customers into clusters to run targeted campaigns

## Approach

Customer segmentation can be grouped into 3 types i.e. demographic segmentation, attitudinal segmentation and behavioural segmentation. The idea is to segment customers based on when their last purchase was, how often they’ve purchased in the past, and how much they’ve spent overall. All three of these measures have proven to be effective predictors of a customer's willingness to engage in marketing messages and offers. In this senario, since we have customers purchase history available with us its easy to move forward with behavioral segmentation. In B2C business, RFM i.e. Recency-Frequency-Monetary are the most commonly used metrics to measure a customer's purchase behaviour. Upon deriving the RFM metrics, K-means algorithm is used to perform clustering.

<RFM Image>

### Steps Involved

1. Overview and understanding of data
2. Data preprocessing
3. Data preparation for modeling
4. Cluster assignment using K-means clustering
5. Recommendations

# Getting Started

## Installations

Before starting executing the jupyter notebook, execute below commands in terminal for setting up the virtual environment and installing packages:

1. Create virtual environment

```
python3 -m venv env
```

2. Activate newly created virtual environment `env`

```
env/Scripts/activate.bat
```

3. Execute below command to install python packages used in this project

```
pip install requirement.txt
```

## Overview and understanding of data

Getting familiar with dataset and performing discreptive statistics to identify inconsistensis in dataset.

## Data preprocessing

Dealing with missing values and insconsistensis in data to make the data uniform. Formatting columns to required datatypes for easier data transformations.

## Data Prepeparation

Before we start with data modelling, we have to group transaction at customer level and calculate their R-F-M metrics. Once metrics are calculated data preparation piplines are create for scaling and PCA.

## Cluster assignment using K-means clustering

Choosing right number of clusters
<Elbow curve>

Once cluster assignment has been made, below are the characteristics of clusters that were observed:

- Cluster 0 contains the customers who generate the least revenue and are not frequent, most likely because these were one-time customers. Hence they can be labeled as Slipping.
- Cluster 1 seems to have the most loyal customers, as they bring the most revenue and are often the most frequent customers.
- Cluster 2 customers seem promising as it consists of frequent buyers, however revenue generation is not as high as Loyal customers.

<Cluster Profiling>

Finally after cluster profiling below was the distribution across clusters:

<cluster Distbn>

## Recommendations

After segmenting customers into loyal, slipping and promising it empowers business to run personalized, high performing campaigns and preserves profit margin. Below are few recommedations or targeted stratergies for each customer segment:

- **Loyal** - Loyalty programs are effective for these repeat visitors. Advocacy programs and reviews are also common X1X strategies. Lastly, consider rewarding these customers with Free Shipping or other like benefits.

- **Promising** - Focus on increasing monetization through product recommendations based on past purchases and incentives tied to spending thresholds.

- **Slipping** - Customers leave for a variety of reasons. Depending on your situation price deals, new product launches, or other retention strategies

# Contacts

[Linkedin](https://www.linkedin.com/in/raj-praveen-pradhan-306625101/)<br>
Email : [rppradhan310@gmail.com](rppradhan310@gmail.com)
