# Capstone_Arvato_Customer_Acquisition

## Installation

There should be no necessary libraries since all necessary packages are included at the beginning of the notebook.

## Motivation

In today’s data-driven world, businesses are leveraging advanced programming techniques to gain a deeper understanding of their customers and optimize their acquisition strategies.
In the capstone project of Udacity’s Data Scientist Nanodegree demographic data is used to gain insigits about the customer base and determine whether a person is more likely to become a customer of a mail-order company or not.

In the first part of the project the focus was laid on finding differences between the demographic data of the general population and the data of the customer base in order to get a general idea what a typical customer looks like.

In the second Part a Machine Learning Algorithm is used to predict potential new customers.

## Results

As in most Data Science tasks the main part of the task at hand was the data preprocessing in order to analyze the data properly. In order to retain a clean and scaled dataset a lot of assumptions had to be made. 
The following cleaning steps had to be performed to the datasets:

Drop undescribed features
Convert unknown Value flags to NaN Values
Drop columns with too many missing values
Drop rows with too many missing values
Re-encode or drop categorial values
Impute and Scale the Dataset

After this, Using PCA and KMeans Clustering we were able to categorize individuals that form the core customer base of a mail-order company. 
With the provided demographics data the characteristics of the customer base could be identified.

Finally we analyzed the performance of different Machine Learning models, to predict which individuals from a marketing campaign would most likely convert into customers.

## Addtional information

If you want to further dive into the topic the findings are presented in this blogpost:
https://medium.com/@dennis.kellner93/optimizing-customer-acquisition-with-machine-learning-7f134849bcfd
