# [View Presentation Here!](</Regression Presentation.pdf>)

# Modeling overall satisfaction scores of university courses with other course statistics

*Matteo Fortier*

## Abstract

The goal of this project was to produce a regression model that can best interpret a relationship for overall satisfaction and a model that can best predict overall satisfaction. The purpose of the analysis was to provide universities aspects of a course which can be focused on to improve overall satisfaction. Data from discoveruni.org was web scrapped to allow exploration of these relationships. SKLearn libraries were used to explore the different regression models that could be used. Results were visualised using matplotlib and seaborn. 

## Design

Universities (in the UK) receive a lot of per course feedback from students via the national student survey, along with an overall satisfaction score for the course. These scores are also publicly available through various websites that help prospecting students choose the universities they want to study at. Consequently, universities have an icentive to keep those overall satisfaction scores high. It is unlikely however, that many universities are able to improve all aspects of a course all at once. Thus it is valuable to model which aspects of a course impacts the overall score the most. 

## Data

The project scraped 1 dataset from discoveruni.org. The dataset included data from 442 universities (course providers) and 35219 courses, some courses having multiple subjects. This resulted in 47,000 rows of data for analysis and modeling. The dataset had 38 feature variables along with the target variable. The feature variables were primarily numeric with some being categorical. However after exploration none of the categorical features were used, even after feature engineering was conducted on them. The dataset was not optimal in certain regards. Namely, the distribution of the target data was centred towards higher values. Hence, models performed better towards higher value targets.

## Algorithms

SKLearn linear models were explored including linear regression, lasso regression and ridge regression. Standard scaler was used for the regularization models. Feature engineering was also conducted to explore how to best model the target variable. This included categorical feature manipulation and feature interactions. However no categorical features were included in the final models. Train test split was used to empirically test the models against a test set. R2 and MAE were the main metrics used to compare models. These metrics were also used in feature selection along with pairplots and correlation analysis. 

## Tools

Selenium was initially used to scrape the HREFS of all courses from 23 dynamic pages. BeautifulSoup was then used to scrape the course pages. The data was iteratively saved onto a SQLite database and SQLAlchemy was used to ingest the data for EDA and Regression. Pandas and SKLearn were used for the EDA and regression modeling. Finally results were visualised using matplotlib and seaborn. 

## Communication

The project used google slides for the presentation and the previously mentioned visualisation libraries for the visuals. 
