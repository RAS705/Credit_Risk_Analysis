# Credit Risk Analysis

## Introduction to the analysis

LendingClub, a peer-to-peer lending services company, has asked that we help Jill their lead machine learning analyst. They have asked Jill and us to build a machine learning model which will help evaluate the credit risk of a person asking for a loan.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use different techniques to build and evaluate models for evaluating credit risk.

## Results

Jill asked us to utilize a number of methods to build the machine model utilized to help evaluate the loan applicants credit risk.

The following methods were utilized to build models for predicting the credit risk of an applicant:

<table>
<tr>
<td>Balanced Accuracy</td>
<td>What is the average percentage of correct predictions by class?</td>
</tr>
<tr>
<td>Precision</td>
<td>What total percent of your predictions were correct?</td>
</tr>
<tr>
<td>Recall</td>
<td>What percent of the positive cases did you catch?</td>
</tr>
<tr>
<td>F1 Score</td>
<td>What percent of positive predictions are correct?</td>
</tr>
</table>


1. Random Over Sampling
 	- accuracy score 65.14
 	- Precision: .99
 	- Recall: .61  
 	- F1: .75
2. SMOTE Over Sampling
	- accuracy score 65.66
	- Precision: .99
 	- Recall: .69
 	- F1: .81
3. Cluster Centroids
	- accuracy score 65.66
	- Precision: .99
	- Recall: .69
 	- F1: .75
4. SMOTEENN
	- accuracy score 65.66
	- Precision: .99
	- Recall: .69
 	- F1: .81
5. Random Forest Classifier
	- accuracy score 50.00
	- Precision: .99
	- Recall: .99
 	- F1: .99
6. ADA Boost Classifier
	- accuracy score 50.00
	- Precision: .99
	- Recall: .99
 	- F1: .99

## Analysis

After reviewing our different machine models some interesting things showed up in the results. First, all of the models had a precision of .99. The other interesting thing is that the balanced accuracy scores for the models weren't as positive as the accuracy. They ranged between .50 and 65.66.

The real test of these models is the the F1 score. The different models ran from a low of .75 to a high of .99 for their F1 scores.

If we review the data a little, we find the following:

<table>
<tr>
<td>Low-Risk</td>
<td>101 applicants</td>
</tr>
<tr>
<td>High-Risk</td>
<td>17104 applicants</td>
</tr>
</table>

This has made some of the analysis truly challenging and has led to large differences in balanced accuracy scores and precision scores. while a number of the models seem to work for high-risk applicants well, they don't work well for low-risk applicants. With this in mind, I would recommend more research to find a more suitable approach to building the model for this dataset.