
# Welcome to the King County Housing Project Repo!
# By Joe Sanchez




## Introduction

Hello and welcome to my project repo!
My name is Joe Sanchez and I'll be walking you through the directory, as well as give you an introduction to this project!

To start, this project is to test how well I can accurately predict housing prices and its features!
The King County Housing dataset will be analyzed to make these predictions. After it has been cleaned and processed of course.
The dataset contains all types of features you'd normally find while looking for houses, such as bathrooms, bedrooms, and square footage! So it is now my responsibility to use these features and advanced statistics to build a Model that predicts the prices.

Now, before going forward, here is a directory of this repo!

## Directory

* The King County dataset is located: [here](kc_house_data.csv)
* A copy of the column names and their descriptions for the dataset are located: [here](column_names.md)
* The Read Me file (incase you need to come back) is located: [here](README.md)
* The preprocessing of the dataset is located: [here](Preprocessing.ipynb)
* The final modeling of the dataset is located: [here](Final-Modeling.ipynb)
* The preprocessed dataframe is located: [here](prepro_df.csv)
* The final model dataframe is located: [here](final_model_df.csv)

**Please keep in mind that there are two notebooks! One for preprocessing and one for final modeling!

## Business Approach/Goal

Now there isn't a given scenario for this project, so I decided to go with the idea that I am building a multiple linear regression model to predict housing costs for a real estate firm. My goal is to accurately predict the costs of housing features, and after, informing real estate agents of my findings that they can then use to help their clients buy or sell houses.

I want to give real estate agents the tools to potentially out play their competitors by offering housing cost predictions at 95% accuracy using statistics and data analytics. Typically when someone wants to sell their home, they get an appraisal to know the value of their home. However, buyers don't always trust a sellers appraisal. That's where the real estate agent can come in. Although real estate agents aren't official home appraisers, that doesn't mean they can't use the tools home appraisers have.
And thats where I come in. 


## Methodologies Used

* Multiple Linear Regression
* Data cleaning (dealing with outliers and null values)
* Data processing: Dealing with categorical values (creating dummy variables, binary format conversions)
* Data processing: Dealing with non-categorical values (normalizing and dealing with multicollinearity)
* Ordinary Least Squared (OLS) Modeling
* Validating regression assumptions (linear, normality, qqplots, heteroscedasticity)
* Plots used: regplot, boxplot, barplot, histplot, qqplot, scatterplot



## Limitations

The King County Dataset has a wide variety of column features, as well as columns values! Which is great to work with. After further analysis, limitations have been set to fit the OLS Model. Reasons being, there were major outliers in some of the columns as a result of wide variety values. These outliers add complexity and can potentially add heavy skewness to our model. To make sure I can be as accurate as possible, limitations were applied, which alowed me to focus on what would be considered the middle class demographic.

Limitations include:

* Price of houses < 1,000,000
* Bathrooms       < 6
* Bedrooms        < 7
* Square footage  < 6,000
* Floors          < 3

## Sneak Peak

Here's a quick overview of my work in building a multiple linear regression model to predict the prices of home in King County.

![Distplot Before Limitation](price-over-1m.png)

## Questions

Here are a few questions that came up during my modeling process.

* How does the number of bathrooms impact housing price?

* What is the difference between condition and grade? How do they affect the prices of homes?

* What are the most significant features real estate agents need to know about?


## Recommendations

There are many ways to go about building a multiple regression model using the King County Dataset.
Many avenues were explored, and many avenues have yet to be discovered. The dataset contains wide variety of features, however I was not able to add every single one, nor fully clean and process every single one.
Here's a list of features that needed to be more looked at for future work:

* - Lat and Long are both individual columns of the dataset. Combining these two columns respectively may result in significant results.

* - Date is included for each house. The date intels when the house was bought. Further analysis may prove beneficial to the R^2 value.

* - Zipcode was also included with each house. Although it's not common for home buyers to research zipcodes specifically, the feature may show underlying significance to the overall model.

## Conclusion

Thank you so much for reviewing this Read Me, and I hoped this helped give an overall summary of what this repo contains.



