# Credit_Risk_Analysis by Ketaki
## Overview of the analysis:
This project is to help LendingClub analyze the credit risk for loans to their customers based on their credit card dataset.  This dataset is analyzed using imbalanced-learn and scikit-learn libraries to build and evaluate six models using resampling that predict credit risk. Based on the evaluation of these models, we can select a suitable one to be actually used for this project.
## Results: 
The six models used for this project are:
Models based on Resampling:
1. Random Oversampling
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/Random%20Oversampling%20Acc.PNG)
2. SMOTE
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMPOTE%20Acc.PNG)
3. Clustered Centroid
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20CR.PNGG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/ClusteredCentroids%20Acc.PNG)
4. SMOTEEN 
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/SMOTEEN%20aCC.PNG)
 Ensemble Learners:
5. Balanced Random Forest Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Classification%20Report.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/BalancedRandom%20Acc.PNG)
6. Easy Ensemble AdaBoost Classifier
- ![Classification Report](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20CR.PNG)
- ![Accuracy](https://github.com/ketpradh/Credit_Risk_Analysis/blob/main/Resources/EasyEnsemble%20Acc.PNG)


## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
Based on the above evaluation for the mdoels, we find that the Ensemble learners perform better on the dataset.
