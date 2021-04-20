![GitHub Repo stars](https://img.shields.io/github/stars/rppradhan08/ecom-rfm-segmentation)
![GitHub forks](https://img.shields.io/github/forks/rppradhan08/ecom-rfm-segmentation?color=green)
![contributors-shield](https://img.shields.io/github/contributors/rppradhan08/ecom-rfm-segmentation)
[![LinkedIn][linkedin-shield]](https://in.linkedin.com/in/raj-praveen-pradhan-306625101)

[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555

<h1 align="center">
  <br>
  <a href="https://github.com/rppradhan08/ecom-rfm-segmentation"><img src="https://raw.githubusercontent.com/rppradhan08/ecom-rfm-segmentation/master/images/Customer-segmentation.png" alt="Customer Segmentation" width="400" style="border-radius: 50px"></a>
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
  - [Data Preprocessing](#data-preprocessing)
  - [Data Preparation](#data-preparation)
  - [Cluster assignment using K-means clustering](#cluster-assignment-using-k-means-clustering)
  - [Recommendations](#recommendations)
- [Contacts](#contacts)

# About the Project

In this project, I have used [E-Commerce dataset](https://www.kaggle.com/carrie1/ecommerce-data) from Kaggle to perform RFM Analysis and used K-means clustering to segment customers into different clusters based on their behavioral characteristics.

## Business Problem

As a manager of the online store, you would want to group the customers into different clusters, so that you can make a customized marketing campaign for each of the groups. You would have to decide what the important business criteria are on which you would want to segregate the customers. This is a transnational data set that contains all the transactions occurring between 01/12/2010 and 09/12/2011 for a UK-based and registered non-store online retail. The company mainly sells unique all-occasion gifts. Many customers of the company are wholesalers.

### Task

- Decide the important business criteria to segregate the customers
- Group customers into clusters to run targeted campaigns

## Approach

Customer segmentation can be grouped into 3 types i.e. demographic segmentation, attitudinal segmentation, and behavioral segmentation. The idea is to segment customers based on when their last purchase was, how often they’ve purchased in the past, and how much they’ve spent overall. All three of these measures have proven to be effective predictors of a customer's willingness to engage in marketing messages and offers. In this scenario, since we have the customer's purchase history available with us it's easy to move forward with behavioral segmentation. In B2C business, RFM i.e. Recency-Frequency-Monetary are the most commonly used metrics to measure a customer's purchase behavior. Upon deriving the RFM metrics, the K-means algorithm is used to perform clustering.

<div align="center">
<img src="https://raw.githubusercontent.com/rppradhan08/ecom-rfm-segmentation/master/images/rfm-analysis.png" alt="RFM Segmentation" width="75%" style="border-radius: 10px">
</div>

### Steps Involved

1. Overview and understanding of data
2. Data preprocessing
3. Data preparation for modeling
4. Cluster assignment using K-means clustering
5. Recommendations

# Getting Started

## Installations

Firstly, execute the below commands in the terminal for setting up the virtual environment and installing packages:

1. Create a virtual environment

```
python3 -m venv env
```

2. Activate newly created virtual environment `env`

```
env/Scripts/activate.bat
```

3. Execute the below command to install python packages used in this project

```
pip install requirement.txt
```

## Overview and understanding of data

Getting familiar with the data and performing descriptive statistics to identify inconsistencies in the dataset.

## Data Preprocessing

Dealing with missing values and inconsistencies in data to make the data uniform. Formatting columns to required data types for easier data transformations.

## Data Preparation

Before we start with data modeling, we have to group transactions at the customer level and calculate their R-F-M metrics. Once metrics are calculated data preparation pipelines are created for scaling and dimensionality reduction.

## Cluster assignment using K-means clustering

Choosing the appropriate number of clusters depends on business understanding and domain expertise. However in this case we use techniques like Elbow curve and silhouette analysis for determining the optimal number of clusters.

<div align="center">
<img src="https://raw.githubusercontent.com/rppradhan08/ecom-rfm-segmentation/master/images/elbow_curve.PNG" alt="Elbow curve"  style="border-radius: 10px" width=35%>
</div>

After cluster assignment, the following are the unique characteristics traits that were observed:

- **Cluster 0** contains the customers who generate the least revenue and are not frequent, most likely because these were one-time customers. Hence they can be labeled as Slipping.
- **Cluster 1** seems to have the most loyal customers, as they bring the most revenue and are often the most frequent customers.
- **Cluster 2** customers seem promising as it consists of frequent buyers. However, revenue generation is not as high as Loyal customers.

<div align="center">
<img src="https://raw.githubusercontent.com/rppradhan08/ecom-rfm-segmentation/master/images/cluster-profile.PNG" alt="cluster profiling"  style="border-radius: 10px" width=55%>
</div>

Finally, after cluster profiling below was the distribution of customers across clusters:

<div align="center">
<img src="https://raw.githubusercontent.com/rppradhan08/ecom-rfm-segmentation/master/images/cluster-distn.PNG" alt="target distribution"  style="border-radius: 10px" width=35%>
</div>

## Recommendations

After segmenting customers into loyal, slipping, and promising it empowers businesses to run personalized, high-performing campaigns and preserves profit margin. Below are a few recommendations or targeted strategies for each customer segment:

- **Loyal** - Loyalty programs are effective for these repeat visitors. Advocacy programs and reviews are also common X1X strategies. Lastly, consider rewarding these customers with Free Shipping or other like benefits.

- **Promising** - Focus on increasing monetization through product recommendations based on past purchases and incentives tied to spending thresholds.

- **Slipping** - Customers leave for a variety of reasons. Depending on your situation price deals, new product launches, or other retention strategies.

# Contacts

Socials : [Linkedin](https://www.linkedin.com/in/raj-praveen-pradhan-306625101/)<br>
E-mail : [rppradhan310@gmail.com](rppradhan310@gmail.com)
