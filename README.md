# Vehicle-Insurance-Prediction

## Data Description

ClaimNumber : Unique policy identifier

DateTimeOfAccident : Date and time of accident

DateReported : Date that accident was reported

Age : Age of worker

Gender : Gender of worker

MaritalStatus : Martial status of worker. (M)arried, (S)ingle, (U)unknown.

DependentChildren : The number of dependent children

DependentsOther : The number of dependants excluding children

WeeklyWages : Total weekly wage

PartTimeFullTime : Binary (P) or (F)

HoursWorkedPerWeek : Total hours worked per week

DaysWorkedPerWeek : Number of days worked per week

ClaimDescription : Free text description of the claim

InitialIncurredClaimCost : Initial estimate by the insurer of the claim cost

UltimateIncurredClaimCost : Total claims payments by the insurance company. This is the field you are asked to predict in the test set.

## Problem Statement
To predict the Total Claims Payments by the insurance company.

### The approach to work on the dataset in as follows:

1. Importing the libraries that was needed.

2. Pre-Processing

In the pre-processing I wrote codes to obtain basic information on the dataset such as data description,data shape, whether or not if there are any duplicate values or missing data in the dataset. As some of the columns had some missing data I treated them using mean and mode imputation. Following that I worked on binning some of the data columns into small intervals and replaced it by a general value calculated for that bin . This is done in order to understand those columns further more and analyse them.

3. Exploratory Data Analysis

After data pre-processing I focused on exploring the data.

I examined the link between different variables using histogram(for numerical variables) and countplots(for categorical variables). Using Correlation plots, I tried to understand the relationship between all the numerical variables with each other as well as the target variable.

4. Outlier Analysis

Using boxplots, I looked for outliers. Outliers were handled using a function.

5. Machine Learning Models

I experimented with three different models: Linear regression,Random Forest, decision tree regressor, gradient boost and light gradient boost

6. Result

Out of these 5 I selected light gradient boost as it was giving the least root mean squared error (RMSE).
