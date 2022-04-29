# LendingClub Dataset Analysis

### **Overview of the LendingClub Dataset Analysis**
The purpose of this analysis is to assess the reviews from members of the paid Amazon Vine review program. From the available datasets, the Video Games dataset was assessed.

## Results


The results for each model are as follows:


### RandomOverSampler:

	Balanced Accuracy Score: 	0.63
	Precision Score: 		0.99
	Recall Score: 			0.69

![Figure 1](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig1_RandomOverSampler.png)
**_Figure 1_:** RandomOverSampler Summary Statistics

	
### SMOTE:
	Balanced Accuracy Score: 	0.66
	Precision Score:		0.99
	Recall Score:			0.66
	
![Figure 2](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig2_SMOTE.png)
**_Figure 2_:** SMOTE Summary Statistics
	
### ClusterCentroids:
	Balanced Accuracy Score: 	0.53
	Precision Score:		0.99
	Recall Score:			0.45

![Figure 3](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig3_ClusterCentroids.png)

**_Figure 3_:** ClusterCentroids Summary Statistics


### SMOTEENN
	Balanced Accuracy Score: 	0.64
	Precision Score: 		0.99
	Recall Score:			0.57

![Figure 4](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig4_SMOTEENN.png)

**_Figure 4_:** SMOTEENN Summary Statistics

### BalancedRandomForrestClassifier:
	Balanced Accuracy Score: 	0.79
	Precision Score:		0.99
	Recall Score:			0.91

![Figure 5](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig5_BalancedRandomForestClassifier.png)

**_Figure 5_:** BalancedRandomForrestClassifier Summary Statistics

### EasyEnsembleClassifier:
	Balanced Accuracy Score: 	0.93
	Precision Score:		0.99
	Recall Score:			0.94

![Figure 6](https://github.com/CR-HSDC/cryptocurrencies/blob/main/resources/Fig6_EasyEnsembleClassifer.png)

**_Figure 6_:** EasyEnsembleClassifier Summary Statistics



## Summary 

A positivity bias is observed for the Vine reviews. There is a difference of 12.4% between the Vine 5-Star reviews (51.1%) and non-Vine 5-Star reviews (38.7%), this difference is statistcally significant. 

An additional analysis to support the claim of positivity bias, could be to analyze the scoring trends in general. Starting with the overall average score for both categories, it could be assessed if the overall score is higher for the Paid reviews. Additionally, the standard deviation for both averages could be assessed to see if there is lesser variability in the Paid reviews group, thus a higher inclincation towards positive reviews, this could be indicated by a lower standard deviation than for the non-paid group.

Additionally, statistics could be assessed at each discrete score point (e.g. 1 star, 1.5 star etc..) to examine if there bias is any particular score rating.











