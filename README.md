# Sampling-Assignment
# Exploring Sampling Techniques in Credit Card Fraud Detection
In this Python script, we implemented diverse sampling methods on a credit card fraud detection dataset and subsequently tested multiple machine learning models to determine the most effective combination of model and sampling technique based on accuracy.

We employed the following 5 sampling techniques:

1.Random Under Sampler (Designated as Sampling1)
2.Random Over Sampler (Designated as Sampling2)
3.TOMEK links (Designated as Sampling4)
4.SMOTE (Designated as Sampling3)
5.Near Miss (Designated as Sampling5)

The Sample size was calculates using the following formula: n = Z^2(p(1 – p)/m^2) where: n = sample size Z = z-value (for 98% confidence interval, Z = 4) p = proportion of the minority class (taken as 0.5 for a balanced dataset) m = margin of error (taken as 0.1 for a sample size of 1000)

Following 5 models were applied on the sampled dataset:

1.Decision Tree Classifier (Designated as M1)
2.Random Forest Classifier (Designated as M2)
3.KMeans (Designated as M3)
4.Support Vector Classifier (SVC) (Designated as M4)
5.Extra Tree Classifier (Designated as M5)
Upon executing the code, we obtained the following results. The table cells represent the accuracy of each applied model using the corresponding sampling technique.

# Output  

        Sampling1  Sampling2   Sampling3   Sampling4   Sampling5

    M1    37.50       48.71       48.71       48.71       33.62   
    M2    79.31       97.84       98.28       97.84       10.34   
    M3    68.97       99.57       99.57       99.57       56.90   
    M4    58.62       99.57       99.57       99.57       40.95   
    M5    65.95       99.57       99.57       99.57       34.48   
# Result

From the table, it is evident that the highest accuracy of 99.57% was achieved with the following combinations:

1.Decision Tree with Random Over Sampler, SMOTE, and TOMEK
2.Random Forest Classifier with Random Over Sampler, SMOTE, and TOMEK
3.KMeans Classifier with Random Over Sampler, SMOTE, and TOMEK
4.Support Vector Classifier with Random Over Sampler, SMOTE, and TOMEK
5.Extra Tree Classifier with Random Over Sampler, SMOTE, and TOMEK

Hence, the sampling models Random Over Sampler, SMOTE, and TOMEK demonstrate superior performance.
