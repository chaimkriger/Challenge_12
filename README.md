# Credit Risk Report

## Analysis Overview 

In this Readme, I will describe the analysis I completed for the machine learning models used in this Challenge. 

* The purpose of my analysis is to create a machine learning model that can accurately predict the credit worthiness of borrowers.
* I use a dataset of historical lending activity from a peer-to-peer lending service company to build a model that can help me predict if a borrower will default on a loan or not.
* Credit risk poses a classification problem that’s inherently imbalanced. This is because healthy loans easily outnumber risky loans. The challenge is to help the model remove bias tendencies so that the model won't classify every borrower as healthy. In my analysis, I use various techniques to train and evaluate models with imbalanced classes. 
* At first, I use an ordinary LogisticRegression model to fit the training data and predict the testing data. In doing so, I find that although the model predicts what would appear to be excellent results in the precision and recall catagories, it can be damaging to my company if I even allow one borrower who will default to slip through the cracks of my model. Therefore, with a recall of only 91, I understand that I cannot use this model on future testing data. My solution to this problem is to over-sample the data. This means that my model will create duplicate rows of borrowers who defaulted in the past, which removes all bias tendencies from the model. When I run the predictions again, I find that by over-sampling the data, I can improve my recall up to 99! Although the precision of the model drops by one point, the recall is more important to me when it comes to lending money to borrowers. Overall, I'm pretty comfortable with a 99% success rate in filtering out borrowers who may default on loans.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
   Model 1 Accuracy: 95.2%
   
   Precision for the healthy loans: 100% 
   
   Precision for the high-risk loans: 85%
   
   Recall for the healthy loans: 99%
   
   Recall for the high-risk loans: 91%
   ![screenshot of model 1 report](/")

* Machine Learning Model 2:
   Model 2 Accuracy: 99.3%
   
   Precision for the healthy loans: 100% 
   
   Precision for the high-risk loans: 84%
   
   Recall for the healthy loans: 99%
   
   Recall for the high-risk loans: 99%
   ![screenshot of model 2 report](/Screenshot (39).png")

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* After reviewing the results from both of my models, I've come to the firm conclusion that model 2, the model with the resampled data, is the model I would recommend in this scenario. The reason is quite simple. As a lender, I'm more focused on filtering out high-risk loans than getting every healthy loan correct. It is more important to me to lose a few clients here and there, than to lend money to a borrower who may default.



