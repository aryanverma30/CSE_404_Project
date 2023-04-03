# CSE_404_Project


We experimented with different machine learning models including a Decision Tree, SVM, Perceptron model, Logistic Regression, and Random Forest. 

The Decision Tree model achieved an accuracy of 0.813 on the training dataset and an evaluation accuracy of 0.814 on the test dataset using an 80:10:10 train-validation-test split. This indicates that the model performed reasonably well in predicting the target variable.

The Random Forest model achieved an accuracy of 84.1% on the training dataset and an evaluation accuracy of 83.8% on the test dataset using an 80:10:10 train-validation-test split. The Random Forest model performed better than the Decision Tree model, but both overall reasonably predicted the target. 

The Logistic Regression model performed but when constructed using K-Folds Cross Validation, with an accuracy score of 84.7%. Conducting 100 random 80-20 train-test splits of the data results in a mean accuracy of 84.67%. A singular train-test-validation split results in corresponding 85%-84.6%-82.6% accuracy scores.

The SVM and Perceptron models performed the worst of the five, with accuracies of 78.8% and 77.3%, respectively. Given all of these results from all five models, we’ve decided that we’ll take a closer look at the Random Forest and Logistic Regression models as on average those two models performed the best.

The importance of features in a machine learning model represents the contribution of each feature to the decision-making process. These features varied through the models as the nature of each model was significantly different, but in a general sense, our analysis revealed that these features 'marital-status_ Married-civ-spouse', 'age', 'capital-gain', and 'hours-per-week' were the most important/deciding features. Other features such as 'capital-loss', 'education_ Bachelors', 'occupation_ Prof-specialty', and 'occupation_ Exec-managerial' had moderate importance as well. However, some features such as 'workclass_ Without-pay' and 'occupation_ Armed-Forces' had none or little to none importance, indicating that they had no significant contribution to the decision-making process of the model.
