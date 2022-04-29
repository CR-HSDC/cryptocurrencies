# LendingClub Dataset Analysis

### **Overview of the LendingClub Dataset Analysis**
The purpose of this analysis is to assess the accuracy of loan default predictions, using the LendingClub Dataset, using a variety of machine learning models. 

The accuracy and precision was assessed for the following models:

* RandomOverSampler
* SMOTE
* ClusterCentroids
* SMOTEENN
* BalancedRandomForrestClassifier
* EasyEnsembleClassifier


## Results


The results for each model are as follows:


### RandomOverSampler:

* **Balanced Accuracy Score:** 	0.63 (Average)
* **Precision Score:** 		0.99 (Average), 0.01 (High Risk), 1 (Low Risk)
* **Recall Score:** 		0.69 (Average), 0.56 (High Risk), 0.69 (Low Risk)

![Figure 1](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig1_RandomOverSampler.png)

**_Figure 1_:** RandomOverSampler Summary Statistics

	
### SMOTE:
* **Balanced Accuracy Score**: 	0.66 (Average)
* **Precision Score**:		0.99 (Average), 0.01 (High Risk), 1 (Low Risk)
* **Recall Score**:		0.66 (Average), 0.67 (High Risk), 0.66 (Low Risk)
	
![Figure 2](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig2_SMOTE.png)

**_Figure 2_:** SMOTE Summary Statistics
	
### ClusterCentroids:
* **Balanced Accuracy Score:** 	0.53 (Average)
* **Precision Score:**		0.99 (Average), 0.01 (High Risk), 1 (Low Risk)
* **Recall Score:**		0.45 (Average), 0.61 (High Risk), 0.45 (Low Risk)

![Figure 3](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig3_ClusterCentroids.png)

**_Figure 3_:** ClusterCentroids Summary Statistics


### SMOTEENN
* **Balanced Accuracy Score:** 	0.64 (Average)
* **Precision Score:** 		0.99 (Average), 0.01 (High Risk), 1 (Low Risk)
* **Recall Score:**		0.57 (Average), 0.7 (High Risk), 1 (Low Risk)

![Figure 4](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig4_SMOTEENN.png)

**_Figure 4_:** SMOTEENN Summary Statistics

### BalancedRandomForrestClassifier:
* **Balanced Accuracy Score:** 	0.79 (Average)
* **Precision Score:**		0.99 (Average), 0.04 (High Risk), 1 (Low Risk)
* **Recall Score:**		0.91 (Average), 0.67 (High Risk), 0.91 (Low Risk)

![Figure 5](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig5_BalancedRandomForestClassifier.png)

**_Figure 5_:** BalancedRandomForrestClassifier Summary Statistics

### EasyEnsembleClassifier:
* **Balanced Accuracy Score:** 	0.93 (Average)
* **Precision Score:**		0.99 (Average), 0.07 (High Risk), 1 (Low Risk)
* **Recall Score:**		0.94 (Average), 0.91 (High Risk), 0.94 (Low Risk)

![Figure 6](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig6_EasyEnsembleClassifer.png)

**_Figure 6_:** EasyEnsembleClassifier Summary Statistics


## Summary 

A positivity bias is observed for the Vine reviews. There is a difference of 12.4% between the Vine 5-Star reviews (51.1%) and non-Vine 5-Star reviews (38.7%), this difference is statistcally significant. 

An additional analysis to support the claim of positivity bias, could be to analyze the scoring trends in general. Starting with the overall average score for both categories, it could be assessed if the overall score is higher for the Paid reviews. Additionally, the standard deviation for both averages could be assessed to see if there is lesser variability in the Paid reviews group, thus a higher inclincation towards positive reviews, this could be indicated by a lower standard deviation than for the non-paid group.

Additionally, statistics could be assessed at each discrete score point (e.g. 1 star, 1.5 star etc..) to examine if there bias is any particular score rating.











