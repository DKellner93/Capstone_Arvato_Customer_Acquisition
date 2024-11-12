# Capstone_Arvato_Customer_Acquisition

## Installation and libraries

There should be no necessary libraries since all necessary packages are included at the beginning of the notebook.
- numpy: for computing functions
- pandas: for data structures and data analysis tools as well as to read in the data
- scikit-learn: Machine Learning in python
- matplotlib and seaborn: Plots and Graphs
- time: analyze computing times

## Motivation

In today’s data-driven world, businesses are leveraging advanced programming techniques to gain a deeper understanding of their customers and optimize their acquisition strategies.
In the capstone project of Udacity’s Data Scientist Nanodegree demographic data is used to gain insigits about the customer base and determine whether a person is more likely to become a customer of a mail-order company or not.

In the first part of the project the focus was laid on finding differences between the demographic data of the general population and the data of the customer base in order to get a general idea what a typical customer looks like.

In the second Part a Machine Learning Algorithm is used to predict potential new customers.

## Results

As in most Data Science tasks the main part of the task at hand was the data preprocessing in order to analyze the data properly. In order to retain a clean and scaled dataset a lot of assumptions had to be made. 
The following cleaning steps had to be performed to the datasets:

### Drop undescribed features
At first we drop all features that don't have a description since we don't know how to interpret these in the end
### Convert unknown Value flags to NaN Values
As mentioned above, we use the flags for unkown values from the file in order to change these values to NaN values. This way we can better analyze the data and decided wether we have enough information to use the coressponding columns and rows.
### Drop columns with too many missing values
It looks like there is a threshold at around 20% of missing data so we will use this as a dropoff point and cut all columns with more than 20% missing data
### Drop rows with too many missing values
We decided to drop all rows with more than 15% missing values since there seems to be a threshold
### Re-encode or drop categorial values
Depending on the structure of the categorial variables they were either reencoded or dropped
### Impute and Scale the Dataset
Most Machine Learning algorithms can't cope with NaN Values so we fillthese cells with the mean values of their columns which is a common approach to not bias the data. After that we use a Standard Scaler to scale the data which helps to balance the impact of all variables and can help to improve the performance of the ML algorithm

...

After this, Using PCA and KMeans Clustering we were able to categorize individuals that form the core customer base of a mail-order company. 
With the provided demographics data the characteristics of the customer base could be identified.

Finally we analyzed the performance of different Machine Learning models, to predict which individuals from a marketing campaign would most likely convert into customers.

## Addtional information

If you want to further dive into the topic the findings are presented in this blogpost:
https://medium.com/@dennis.kellner93/optimizing-customer-acquisition-with-machine-learning-7f134849bcfd

## Files
- azdias_features_241108.csv: List of features and their corresponding Unknown Values flags
- Arvato Project Workbook.ipynb: Notebook containing all project files

The raw customer data files aren't uploaded due to copyright reasons from Arvato

## Acknowledgements
Must give credit to Arvato Financial Solutions for the data and project idea as well as Udacity for the inspiration. 
Feel free to use the code here as you would like!

