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
![image](https://user-images.githubusercontent.com/90749275/155944117-19fd167e-12c7-4868-bead-9584e383ec6e.png)
>
![image](https://user-images.githubusercontent.com/90749275/155944429-2b934e95-0741-49ad-9a5e-1a663f85d894.png)
>
##### RandomOverSampler
![RandomOver](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/RandomOver.png)
##### SMOTE
![SMOTE](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/SMOTE.png)
##### undersampling ClusterCentroids
![undersample](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/undersample.png)
##### Combination Sampling With SMOTEENN
![combination](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/combination.png)
##### BalancedRandomForestClassifier
![balancerandomforest](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/balancdrandomforest.png)
##### EasyEnsembleClassifier
![EasyEnsemble](https://github.com/WeiTing83/Credit_Risk_Analysis/blob/main/images/EasyEnsemble.png)
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
