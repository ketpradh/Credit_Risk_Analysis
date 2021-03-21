# Credit_Risk_Analysis by Ketaki
## Overview of the analysis:
This project is to help LendingClub analyze the credit risk for loans to their customers based on their credit card dataset.  This dataset is analyzed using imbalanced-learn and scikit-learn libraries to build and evaluate six models using resampling that predict credit risk. Based on the evaluation of these models, we can select a suitable one to be actually used for this project.
## Results: 
For our analysis, we need to have **higher sensitivity(recall) values for the high_risk category** to identify potential high risk customers that might default on their loans.
The six models used for this project are:
Models based on Resampling:
1. Random Oversampling
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Acc.PNG)
- This model has an accuracy of **0.66** with **0.01** precision and **0.74** recall values and f1 score of **0.02** for high_risk category.
2. SMOTE
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMPOTE%20Acc.PNG)
- This model has an accuracy of **0.65** with  **0.01** precision and **0.62** recall values and f1 score of **0.02** for high_risk category.
3. Clustered Centroid
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20Acc.PNG)
- This model has an accuracy of **0.54** with  **0.01** precision and **0.69** recall values and f1 score of **0.01** for high_risk category.
4. SMOTEEN 
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20aCC.PNG)
- This model has an accuracy of **0.64** with **0.01** precision and  **0.72** recall values and f1 score of **0.02** for high_risk category.
 Ensemble Learners:
5. Balanced Random Forest Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Acc.PNG)
- This model has an accuracy of **0.93** with **0.09** precision and  **0.92** recall values f1 score of **0.16** for high_risk category.

6. Easy Ensemble AdaBoost Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20Acc.PNG)
- This model has an accuracy of **0.93** with **0.09** precision and **0.92** recall values and f1 score of **0.16** for high_risk category.


## Summary:
- Based on the above evaluation for the models, we find that the Ensemble learners perform better than the other four models on the dataset in terms of its accuracy. 
- Both, the Balanced Random Forest Classifier model and the Easy Ensemble Classifier Model have accuracy of **0.93** and overall precision of **0.99** and recall of **0.94**.
- **However, for our analysis, we need to have higher sensitivity(recall) values for the high_risk credit data. Hence, we need to have less False Negatives in that category.** We find that both the Ensemble Learners have a high recall for high_risk category of **0.92**, but low precision(**0.09**) low F1 score(**0.16**).
- The otehr four models do not have as high recall as Ensemble Learners but are in the range of **0.62 - 0.74**. However, have very low precision of **0.01** and F1 score **0.02**. 
- Hence, we do not have a model that satisfies the recall and precision needs for the project. However, we can select either the Balanced Random Forest Classifier model or the Easy Ensemble Classifier Model for their high recall values. 

