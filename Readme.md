# Credit Risk Analysis

### **Credit Risk Analysis**
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

![Figure 7](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig7_Summary.png)
**_Figure 7_:** Model Summary Statistics

***Figure 7*** provides a summary of results for all models used in this summary.

Of interest to this analysis, is accurately predicting High Risk lending. High precision should be expected for Low Risk, since these compromise the vast majority of the dataset. 

Of the assessed models, the EasyEnsembleClassifier had the highest sensitivity for High Risk scores at 0.91, however the precision remained low at 0.07, indicating a high number of false positives. The high sensitity and low precision are reflected in the F1 score of 0.14 for the High Risk category.

Implentation of this algorithm to assess lending risk, should be comenserate with the level of risk. Perhaps for higher value lending (e.g. $10 million+), this algorithm could be useful, to determine if further investigation is required into a borrowers credit worthiness. For regular lending, however, the number of falses positives may be burdersome and encumber potential revenue opportunties. 
