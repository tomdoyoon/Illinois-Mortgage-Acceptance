# Illinois-Mortgage-Acceptance

# Abstract

The objective of this project is to provide an independent study on the relationships between various factors of a property, mortgage application, and mortgage applicant to determine trends for successful home ownership in Illinois.

Every year, the  Federal Financial Institutions Examination Council requires institutions to report mortgage loan application and property data for a report mandated through the Home Mortgage Disclosure Act. 

As property costs continue to rise faster than wages, home-ownership seems more like an American dream than an investment or a choice made with preferences.

To understand the factors of successful mortgage applications, the report uses natural language preprocessing, feature engineering,clustering, statistical analysis, and machine learning applications to develop significant conclusions and relationships between selected features.

Applicants who used a top 15 lender from 2020, ranked by loans issued, had a success rate of 94.27% compared to a 89.98% success rate for those who used a lender out of the top 15. Income played a large role, as expected. Incomes greater than or equal to $105K were over 9% more successful than incomes less than or equal to $62K. While one may assume that a larger loan is more risky to the lender which in turn would lead to rejections, the data says otherwise. Mortgage applications for properties valued over or equal to $325K had a 94.9% success rate compared to an 88.27% success rate for properties valued under or equal to $195K. This may not show the full picture, as loan to value seems to be another big factor. Loan to value less than or equal to 80% has a 95.05% success rate, almost 5% higher than a loan to value greater than or equal to 95%. Perhaps the 20% down payment not only saves on the monthly payments, but also increases mortgage application odds?

The goal of the study is to provide insights into correlated factors with successful mortgage applicants in Illinois. This is done through interpreting various features on the 2021 HDMA report, feature engineering fields, and analyzing stratas to determine statistically significant relationships.

# Introduction

Please use the Table of Contents, found below, to navigate the project!

In this project I explore mortgage application data sourced from the 2021 HDMA report. The data can be retrieved and partitioned by state through the FFIEC’s website under HDMA Data Publication. All cleaning was performed in the Jupyter Notebook, uploaded in the repository.

The project is concluded with a classification deep learning model, Up sampled (Oversample from the minority) Random Forest model, Down sampled (Undersample from the majority) Random Forest model, SMOTE (Synthetic Minority Oversampling Technique) Random Forest model, and a regular Random Forest model that all have an objective to estimate if a particular applicant will be successful and receive a mortgage.

# Table of Contents:
- Loan Outcome Analysis: Engineering, cleansing, and analysis related to the Illinois 2021 HDMA reporting data.
- Loan Outcome Model: Models predicting an Illinois applicant's mortgage outcome.

# Observations and Findings
- MSA-MD code 16984 Chicago-Naperville-Evanston has 57.18% of all applicants and is 1% more successful than the rest of the MSA-MD codes.
- Principal occupancy types have a .489% over Investment occupancy types, however, the P Value is 5.8%.
- High property values (>=$325K) have a 6.65% success advantage over low property values (<=$195K)
- 

# Model Evaluations

The outcome of the mortgage application is heavily imbalanced, 92.88% of all applications were successful.

The top performing classification model would be the random forest model with an over sample of the minority, with a macro average F1 score of .93. Prediction of success had a F1 of .99 and prediction of rejection had a F1 of .87. The random forest model, without sampling techniques, performs quite well and has the same metrics as the over sample of the minority random forest model.
