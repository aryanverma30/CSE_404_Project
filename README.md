# CSE_404_Project

Our codes for our Random Forest and Logistic Regression models are found outside of the folder called “All Other Files”, while all of our other codes (including the ineffective models detailed in Project Step 5) are found within the file. In order to run the file, just run the cells in either file in the main directory. Our subdirectory just includes all our files that were used to compile our final two files in the main directory. Also included in our main directory is our learning curve picture. 


Final Model - Random Forest:

We experimented with different machine learning models, including a Decision Tree, SVM, Perceptron model, Logistic Regression, and Random Forest. However, for this project step, we focused only on the Logistic Regression and Random Forest models. After fine-tuning both models and configuring our data to be more optimal, we were able to increase our Random Forest model by around 2%; whereas for the Logistic Regression we were unable to make a significant change. 
Our logistic regression model achieved an initial accuracy of 84.5% and an F1 score of 0.656. This model was built using scikit learn’s basic LogisticRegression tool with no tuning parameters. We used GridSearchCV with a series of different parameters for maximum iterations, solver methods, regularization values, and weight values for the two classes. We used the optimal parameters to build our final model, which achieved an accuracy of 84.6% and an F1 score of 0.661. This model proved to be less effective than the Random Forest model.
We were able to improve the Random Forest model by running a randomized search algorithm that used 3 fold cross validation to find the best set of parameters for our data. What this means is that we experimented with over 4000 possibilities and returned the best set of parameters to make our model as accurate as possible. After finding these parameters, we compared these results to our base Random Forest model and saw some improvements in the accuracy. 


Learning Curve:

The learning curve(which is located in directory as 'Learning_Curve.png') shows how the accuracy of the model improves as the number of training examples increases. The x-axis represents the number of training examples, and the y-axis represents the accuracy of the model. The green line represents the cross-validation score (i.e., the accuracy on the validation set), and the red line represents the training score (i.e., the accuracy on the training set). The shaded regions around the lines represent the standard deviation of the scores.
If the training score is much higher than the cross-validation score, it indicates that the model is overfitting to the training data and may not generalize well to new data. If the training score and cross-validation score are both low, it indicates that the model is underfitting the data and may benefit from more training examples or a more complex model.
It seems that the training score and cross-validation score are both high and relatively close to each other. The training score starts at 0.925 and ends at 0.903, which indicates that the model is not overfitting too much to the training data. The cross-validation score starts at 0.85 and ends at 0.86, which indicates that the model is able to generalize well to new data.Overall, these results suggest that the model is performing well and has achieved a good balance between bias and variance.



Classification Report (F1 Score):

The model seems to perform reasonably well on the adult census income dataset. The F1-score is a weighted average of the precision and recall, with a value between 0 and 1, where 1 is the best possible score.
The F1-score of 0.91 for class 0 (income <=50K) indicates that the model has a high precision and recall for predicting this class. The precision of 0.87 suggests that out of all the predicted samples as belonging to class 0, 87% of them are actually true positives. The recall of 0.95 indicates that out of all the actual samples belonging to class 0, the model correctly predicted 95% of them.
However, the F1-score for class 1 (income >50K) is 0.69, which is much lower than for class 0. This indicates that the model has lower precision and recall for predicting class 1. The precision of 0.80 suggests that out of all the predicted samples as belonging to class 1, 80% of them are actually true positives. The recall of 0.60 indicates that out of all the actual samples belonging to class 1, the model correctly predicted only 60% of them.
Overall, the macro-average F1-score of 0.80 and the weighted-average F1-score of 0.85 suggest that the model performs reasonably well across both classes. 
