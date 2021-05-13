# Deep Learning Regression with Admissions Data

The goal of this project is to create a regression model that predicts the likelihood that a student applying to graduate school will be accpeted based on various application factors (such as test scores).

By analysing the parameters in the graduate admissions dataset I will use TensorFlow & Keras to create a regression model that can evaluate the chances of an applicant being admitted.

## Dataset

The dataset can be found in `admissions.csv` which contains the following columns:

* Serial No.
* GRE Score - test score (out of 340)
* TOEFL Score - test score (out of 120)
* University Rating - Evaluated university rating (out of 5)
* SOP - Statement of Purpose Strength (out of 5)
* LOR - Letter of Recommendation Strength (out of 5)
* CGPA - Undergraduate GPA (out of 10)
* Research - Has reserach experience (either 0 or 1)
* Chance of Admit - Applicants chance of being admitted (ranging from 0 to 1)

The features of the model were all columns except `Serial No.` and `Chance of Admit`. `Chance of Admit` was the labels for the model. 

## Model

* Model was setup using keras sequential with 1 hidden layer with 128 nuerons. 
* The optimizer used was Adam with a learning rate of 0.01.
* epochs was set to 40.
* batch_size set to 1. 


## Results

The results showed very good performance with MSE at around 0.004 and MAE at 0.04.

## Tuning

I tuned some of the hyperparameters i.e. increasing batch size and hiddens layers, but little improvement was observed. 
