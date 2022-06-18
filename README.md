# Venture Funding with Deep Learning

TO BE COMPLETED

# Technologies

This program leverages python 3.7+

To ensure all dependencies are installed and up-to-date, please run the following commands in your terminal once you have cloned the repository to your local machine.
run pip install -r requirements.txt

---

## Installation Guide

1. Copy this repository via the URL (SSH or HTTP)
<img width="907" alt="Screen Shot 2022-04-03 at 3 35 27 PM" src="https://user-images.githubusercontent.com/98444459/161445246-d4eecac4-44ae-452f-8e0c-ebaa9e523908.png">

2. Run a git clone command in your terminal or git bash under the desired local directory
<img width="689" alt="Screen Shot 2022-05-25 at 1 39 17 AM" src="https://user-images.githubusercontent.com/98444459/170187991-6383aedf-cc47-4550-97f8-54262253043e.png">

3. If you receive errors, please review the dependencies above, install them and try again. 

---

## Usage

1. Navigate to the directory in either the Terminal or GitBash. 

2. From the top folder (Challenge_12), launch jupyter lab by typing 'jupyter lab' into Terminal or Gitbash and pressing 'Enter'
<img width="570" alt="Screen Shot 2022-05-08 at 1 56 51 PM" src="https://user-images.githubusercontent.com/98444459/167309092-db3b1a32-49bf-4a3c-a7d7-cc9674d32d38.png">

3. Open the 'credit_risk_resampling.ipynb' notebook and follow the instructions therein.  
<img width="367" alt="Screen Shot 2022-06-12 at 8 22 24 PM" src="https://user-images.githubusercontent.com/98444459/173268248-d01530c1-b951-449b-a263-2a890b582fc9.png">

---
# Credit Report Analysis

## Overview of the Analysis 

The purpose of this analysis is to determine if a model created to validate the likelihood of default of borrowers using two different datasets. The first is an imbalanced dataset, and the second is resampled dataset. The datasets analyzed contained information on loan size, interest rate, debt-to-income ratio, income, derogatory marks, number of accounts and total debt with a final outcome variable of their loan status (approved or rejected). 

In the first dataset, we have 75036 rejected loans and 2500 approved loans. This, of course, is what we consider an imbalanced dataset.
In the second dataset, we have 56271 rejected and the same number of approved loans. This is our resampled dataset. 

For the imbalanced dataset, we split the data into training and testing data. We then instantiated the linear regression model, fit the training data to the model, made predictions for our testing data outcomes and then evaluated performance with a confusion matrix and accuracy score.
For the resampled dataset, we used RandomOverSampler to resample the data, we fit the model using a resample fit function, then we apply a logistic regression to the resampled data, make predictions and evaluate performance with a confusion matrix and accuracy score. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Accuracy Score: 95%
  * Precision: 85%
  * Recall: 91%


* Machine Learning Model 2:
  * Accuracy Score: 99%
  * Precision: 84%
  * Recall: 99%

## Summary
Based on the above scores, I would recommend using the model built with the resampled data. It has a higher accuracy, better score for recall and is close to the same level of precision. The only concern I would express around this model is the fact that the recall score is so high, it has the potential to be overfit. 

## Contributors

Made by:
Ryan Anderson
  Email: m.anderson.ryan@gmail.com
  LinkedIn: https://www.linkedin.com/in/ryan-anderson-57b2b173

---

## License

No licenses are required to run this application