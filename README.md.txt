# **Waze**

# **User Churn Project**

*9 June to 1 September 2023*

Waze is a community driven navigation app that helps millions of users get to where they’re going through real-time road alerts and an up-to-the-moment map.
Typically, high user retention rates indicate satisfied users who repeatedly use the Waze app over time. This project develops a churn prediction model to help prevent churn, improve user retention, and grow Waze’s business. The questions answered in this project were Who are the users most likely to churn? Why do users churn? and, When do users churn? 

This project was part of my Google Advanced Data Analytics Certificate.

**FINDINGS**

It was established that the data is insufficient for reliably predicting user churn and that further granular data is needed on app usage and geography. Given the data, it could be determined that users who are professional drivers and who use the app more in a month are the biggest predictors of whether a user will churn or be retained.

**PROJECT OVERVIEW**

This was a three-stage project, in which I was involved after the first stage.

## **Stage 1: Project proposal** (not involved)

1. Data was imported and explored for useful user churn information
2. A project proposal was accepted by Waze for an in-depth EDA (stage 2), statistical testing (stage 3), and predictive modelling (stages 4 & 5)

## **Stage 2: EDA** (9-12 June 2023)

1. Churn rate is highest for users who didn’t drive using the app much in the last month 
2. Device types had similar churn rates
3. Key conclusion: Statistical tests need to be run on variable classes (e.g., device used) to determine significant relationships with churn

## **Stage 3: Two-sample hypothesis test** (24-28 June 2023)

1. Calculations show that iPhone users have a higher average use of the app compared to Android users
2. However, this difference is not statistically significant
3. Key conclusion: More marketing-relevant data is needed for statistically examining churn by device use and other variables.

## **Stage 4:Logistic regression analysis** (17-20 July 2023)
1. Ran a binomial logistic regression with slightly better than benchmark precision but very low recall
2. Contrary to what was expected from EDA findings, the amount of driving was the second-least-important variable for predicting churn

## **Stage 5: Predictive classification models** (28 August to 1 September 2023)

1. Features of interest were extracted, and a random forest model and a GBM model on predicting user churn were developed and performances compared
2. The GBM outperformed the random forest model, and it had similar levels of precision and accuracy to the logistic regression, with a much better (though still unsatisfactory) recall score
3. The models confirmed the insufficiency of the data and the need for driver-level data collection (e.g., drive times and geographic information) and user interaction with the app (e.g., input a road hazard).
