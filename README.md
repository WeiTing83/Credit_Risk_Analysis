# Credit_Risk_Analysis

### Overview of the loan prediction risk analysis:
We will use supervised machine learning to do credit card
risk analysis. Credit risk is unbalanced classification
problem. Good loans are easily outnumbered risky loans.
Therefore, we evaluate different models to reduce bias and
predict credit risk.
>
### Results:
Because it is imbalance case, the high number of low-risk
population cause its precision are almost 100%. Therefore, I will
evaluate high-risk sensitivity first.
>
Logistic Regression Classifier	
--------------------------------------------				
	|original sampling	|RandomOverSampler|	SMOTE Oversampling	|undersampling	|combination sampling
--------------------------------------------------------------------------------------------------
balanced_accuracy_score|	50%|	63%|	62%|	62%|	63%
-------------------------------------------------------------------------------
precision-high risk|		|1%|	1%|	1%|	1%
-------------------------------------------------------------
sensitivity-high risk|		|62%	|56%	|67%	|68%
------------------------------------------------------------------
F1-high risk|		|2%	|2%	|2%	2|%
----------------------------------------------------
>
 Ensemble Classifiers
--------------------------------------------------------		
	 |BalancedRandomForestClassifier|	EasyEnsembleClassifier
--------------------------------------------------------
balanced_accuracy_score|	77%|	92%
--------------------------------------------------------
sensitivity-high risk|	66%|	89%
---------------------------------------------------
F1-high risk|	6%|	16%
-----------------------------------------------------
precision-high risk|	3%	|9%
---------------------------------------------------------------
>
![RandomOver]()
![SMOTE]()
![undersample]()
![combination]()
![balancerandomforest]()
![EasyEnsemble]()
>
### Summary
The analysis of credit card risk is imbalance case.
Therefore, detecting low population of high risk is super
important. Based on seven models of supervised machine
learning, the data show all of models are lower sensitivity
for high risk of population. Only EasyEnsembleClassifier
looks better than others. Its sensitivity is 89% for high-risk
of population. Utilizing this model could detect low
population in the high risk. However, there is 11% falsely
detected, so it may cause company to miss some business
opportunity. We have two ways to solve this issue. First, we
should look forward another models. Second, we can
establish customer services to revise some falsely
detected.
