# Context: 

Our client is a large **Real Estate Investment Trust (REIT)** based in **New York State, USA**. They **invest** in houses/ apartments/ condos and as part of their business, they attempt to **predict a fair transaction price** for a property **before it is sold**. This is done to calibrate internal pricing models and to 'keep a pulse' on the housing market.

As things stand, they currently employ **independent appraisers** to evaluate a property and to provide an estimate on the price of the property based on the features of that property. However, the drawback of this approach is that the quality of the appraisers can **vary wildly**, and thus, so can their ability to **accurately predict** transaction prices. 

Inexperienced appraisers have, **on average, an error of 70K USD** between the predicted transaction price, and the actual transaction price. 

In order to eliminate any errors between the predicted and actual price, the client would like to replace the services of the appraisers with a machine learning model and they have hired us to develop that.


# Objectives: 

1) Explore the techniques involved in an entire **Machine Learning workflow** from start to finish.

2) Build a real estate pricing model to accurately predict transaction price with a **Mean Absolute Error (MAE) of < 70K USD.**

# Document Structure

We have followed **5 key steps** in our Machine Learning framework:

**Section 1** - Exploratory Analysis: This first step is meant to be quick, efficient and decisive with the end goal of allowing us to get to 'know the data'. We will uncover hints on how to approach data cleaning and which features to select for feature engineering.

**Section 2** - Data Cleaning: Before building any models, we will clean our dataset. In the real world, most datasets are 'messy', i.e., they may contain typos/ duplicate data/ measurement errors and need to be thoroughly cleaned before they can be used for analysis. 

**Section 3** - Feature Engineering: We will create 'new input features' from the existing features within our dataset. Once we go through this process, we will create an 'Analytical Base Table (ABT)' which will represent our dataset after it has been cleaned and augmented through feature engineering.

**Section 4** - Algorithm selection: We will consider three common machine learning regression algorithms, namely: 

- Linear Regression
- Regularized Regression
- Tree Ensemble Methods

**Section 5** - Model Training: We will examine the performance of each of these algorithms on our dataset whilst attempting to avoid overfitting through dataset splitting, pre-processing data pipelines and cross- validation.   

# Executive summary

After considering various linear regression algorithms, we found that the win condition of MAE < 70K USD can be achieved by a Random Forest algorithm. 

The MAE achieved was 68,116 USD and the corresponding R^2 value was 0.57.
