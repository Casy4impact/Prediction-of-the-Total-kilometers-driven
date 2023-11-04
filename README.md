# Prediction-of-the-Total-kilometers-Driven
## Project Objective:
The objective of this project is to develop a predictive model for Waze to estimate the total kilometers driven during a month (driven_km_drives) using supervised learning techniques. The project aims to leverage the available data to create a model that can accurately predict the total kilometers driven by Waze users based on various predictor variables.

## Project Overview:
Waze, a popular navigation application, has contracted 10Alytics to build a predictive model for estimating the total kilometers driven during a month. The model will help Waze gain insights into user behavior and usage patterns, allowing for better service and resource allocation. The project involves exploratory data analysis, model development, and evaluation of different machine learning models to find the best-performing one.

## Data Sources:
•	Data has been provided by Waze, and it includes various predictor variables and the target variable, driven_km_drives.
•	The data includes information about user activity, device types, and retention/churn indicators.

## Data Preprocessing:
## Observations from the exploratory data analysis:
•	Missing data in the label variable.
•	No duplicate records.
•	Presence of outliers 
•	An imbalance in the label variable between retained and churned users.
Data preprocessing steps include handling missing data, outlier detection and treatment, and addressing the class imbalance in the label variable. 

## Below are the predictor variables arranged in order of their predictive power
This was established using relative important chart
1.	duration_minutes_drives: Total duration driven in minutes during the month
2.	n_days_after_onboarding: The number of days since a user sign up for the app
3.	total_sessions: A model estimate of the total number of sessions since a user has onboarded. 
4.	total_navigations_fav1: Total navigations since onboarding to the user’s favorite place 1
5.	sessions: Number of occurrences of users opening the app during the month 
6.	total_navigations_fav2: Total navigations since onboarding to the user’s favorite place 2  
7.	drives: An occurrence of driving at least 1 km during the month   
8.	activity_days: Number of days the user opens the app during the month   
9.	driving_days: Number of days the user drives (at least 1 km) during the month
10.	device_Android: Andriod mobile phone device used to access the app by the user
11.	device_iPhone: iPhone mobile phone device used to access the app by the user
12.	churned: Describe customers who stop using Waze app
13.	retained: Indicate satisfied users who repeatedly use Waze app over time
    
## Machine Learning Method:
Three machine learning models were used in this project:
1.	Linear Regression
2.	Decision Tree
3.	Gradient Boosting

## Evaluation Metrics:
The models were evaluated using the following metrics:
•	R-squared (R2): To measure the proportion of variance explained by the model.
•	Root Mean Squared Error (RMSE): To quantify the prediction error in the target variable.

## Key Insights:
•	Linear Regression performed the best with the highest R-squared (0.4667) and the lowest RMSE (1,839.40).
•	Gradient Boosting had a slightly lower R-squared (0.4588) but still performed well with a reasonable RMSE (1,853.02).
•	The Decision Tree model performed poorly with a negative R-squared and a high RMSE, making it unsuitable for this dataset.

## Benefits: The project offers several benefits:
•	Improved user engagement, leading to longer app usage and more active users.
•	Enhanced user experience based on data-driven improvements.
•	Increased user retention, which can boost Waze's user base and community.
•	Better understanding of user behavior and preferences.

## Business Recommendations:
1.	Waze should consider implementing the Linear Regression model as it performed the best in predicting total kilometers driven. This model can provide valuable insights into user behavior.
2.	The Ridge Regression model, which explained a slightly higher proportion of the variance, could be a good choice for interpretability and avoiding multicollinearity.
3.	Waze should use the predictive model to gain insights into user behavior, make data-driven decisions, and optimize its services and resources.
   
## Conclusions:
The project successfully developed predictive models to estimate total kilometers driven during a month using various machine learning techniques. Linear Regression and Ridge Regression emerged as the top-performing models. These models can help Waze better understand user behavior, optimize its services, and improve user retention. However, it's essential to keep refining and fine-tuning these models as the dataset and user behavior evolve over time.

