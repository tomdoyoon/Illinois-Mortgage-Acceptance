# Illinois-Mortgage-Acceptance

# Abstract

The objective of this project is to provide an independent study on the relationships between various factors of a property, mortgage application, and mortgage applicant to determine trends for successful home ownership in Illinois.

Every year, the  Federal Financial Institutions Examination Council requires institutions to report mortgage loan application and property data for a report mandated through the Home Mortgage Disclosure Act. 

As property costs continue to rise faster than wages, home-ownership seems more like an American dream than an investment or a choice made with preferences.

To understand the factors of successful mortgage applications, the report uses natural language preprocessing, feature engineering,clustering, statistical analysis, and machine learning applications to develop significant conclusions and relationships between selected features.

The goal of the study is to provide insights into correlated factors with successful mortgage applicants in Illinois. This is done through interpreting various features on the 2021 HDMA report, feature engineering fields, and analyzing stratas to determine statistically significant relationships.

# Introduction

Please use the Table of Contents, found below, to navigate the project!

In this project I explore mortgage application data sourced from the 2021 HDMA report. The data can be retrieved and partitioned by state through the FFIEC’s website under HDMA Data Publication. All cleaning was performed in the Jupyter Notebook, uploaded in the repository.

The project is concluded with a classification deep learning model, Up sampled (Oversample from the minority) Random Forest model, Down sampled (Undersample from the majority) Random Forest model, SMOTE (Synthetic Minority Oversampling Technique) Random Forest model, and a regular Random Forest model that all have an objective to estimate if a particular applicant will be successful and receive a mortgage.

# Table of Contents:
- Loan Outcome Analysis: Engineering, cleansing, and analysis related to the Illinois 2021 HDMA reporting data.
- Loan Outcome Model: Models predicting an Illinois applicant's mortgage outcome.




# Observations and Findings


# Model Evaluations

The outcome of the mortgage application is heavily imbalanced, 92.88% of all applications were successful.

The top performing classification model would be the random forest model with an over sample of the minority, with a macro average F1 score of .93. Prediction of success had a F1 of .99 and prediction of rejection had a F1 of .87. The random forest model, without sampling techniques, performs quite well and has the same metrics as the over sample of the minority random forest model.
