# Lungcancer
Classification

### Problem statement
Lung cancer is a malignant tumor that develops from the glands and mucous membrane of the lung tissue and bronchi. 
Every year, about 2.2 million cases of lung cancer are diagnosed in the world, or 11.4% of all detected malignancies. In world statistics, lung cancer ranks second after breast cancer.

The effectiveness of cancer prediction system helps the people to know their cancer risk with low cost and it also helps the people to take the appropriate decision based on their cancer risk status.
The data is collected from the website online lung cancer prediction system .

In this dataset, I will try to use models to predict who is more likely to develop lung cancer. 
To find out what are the risk factors that can be changed in advance and prevent the development of lung cancer.

To train the data I use the models : AdaBoost Classifier, 
                                     Logistic Regression , 
                                     KNeighborsClassifier, 
                                     SVC, 
                                     Decision Tree Classifier, 
                                     RandomForestClassifier, 
                                     XGBClassifier, 
                                     Gaussian.

The dataset is unbalanced so after the first training the prediction is low .
I balance the dataset with Adasyn, then I train again and get high results. 


### Conclusion: 
1. This dataset has 309 rows × 16 columns. It is unbalanced Lung cancer patients 87%, non-positive 13%
2. Lung cancer is almost the same, but more often men. On average, lung cancer occurs between the ages of 56 and 64 years for both men and women, regardless of gender.
3. People who smoke and drink are more likely to develop lung cancer. 
4. Lung cancer occurs more often in people who have chronic disease and persistent anxiety, depression, fatigue. 
5. On unbalanced dataset AdaBoostClassifier, LogisticRegression show the best results.
KNeighborsClassifier, SVC, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, GaussianNB predict weakly and are highly tunable. 
But precision, recall, f1-score metrics show very low results, below 70% or 1%, which indicates that the model is unstable. 
Weakly predict 0 - that the person does not have lung cancer.  As a result, with these scores, it is possible to erroneously diagnose a non-sick person with lung cancer. 
7.  After balancing the data using Adasyn: SVC, KNeighborsClassifier, shows the best and stable result. 
Metrics precision, recall, f1-score also predict above 90%, which shows the reliability of the model. LogisticRegression, AdaBoostClassifier, GaussianNB underfitting. 
Tree-based models RandomForestClassifier, XGBClassifier, DecisionTreeClassifier predict weakly and have overfitting.
