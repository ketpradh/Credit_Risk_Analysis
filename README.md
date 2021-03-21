# Credit_Risk_Analysis by Ketaki
## Overview of the analysis:
This project is to help LendingClub analyze the credit risk for loans to their customers based on their credit card dataset.  This dataset is analyzed using imbalanced-learn and scikit-learn libraries to build and evaluate six models using resampling that predict credit risk. Based on the evaluation of these models, we can select a suitable one to be actually used for this project.
## Results: 
The six models used for this project are:
Models based on Resampling:
1. Random Oversampling
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Acc.PNG)
- This model has an accuracy of **66%** with overall **99%** precision and **59%** recall values.
2. SMOTE
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMPOTE%20Acc.PNG)
- This model has an accuracy of **65%** with  overall**99%** precision and **68%** recall values.
3. Clustered Centroid
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20Acc.PNG)
- This model has an accuracy of **54%** with overall **99%** precision and **40%** recall values.
4. SMOTEEN 
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20aCC.PNG)
- This model has an accuracy of **64%** with overall **99%** precision and **57%** recall values.
 Ensemble Learners:
5. Balanced Random Forest Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Acc.PNG)
- This model has an accuracy of **93%** with overall **99%** precision and **94%** recall values.
6. Easy Ensemble AdaBoost Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20Acc.PNG)
- This model has an accuracy of **93%** with overall **99%** precision and **94%** recall values.


## Summary:
- Based on the above evaluation for the models, we find that the Ensemble learners perform better than the other four models on the dataset in terms of its accuracy. 
- Both, the Balanced Random Forest Classifier model and the Easy Ensemble Classifier Model have accuracy of **93%** and precision of **99%** and recall of **94%**.
- In terms of precision, all six models have similar precision of **99%**. **However, for our analysis, we need to have higher sensitivity(recall) values for the high_risk credit data. Hence, we need to have less False Negatives in that category.** We find that both the Ensemble Learners have a high recall for high_risk category of **92%** and a overall recall of **94%**.
- Hence, we can select either the Balanced Random Forest Classifier model or the Easy Ensemble Classifier Model for this analysis. 

