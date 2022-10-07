# Credit Card Fraud Detection
- The link to the project: 
https://github.com/tiq015UCSD/Credit_Card_Fraud_Detection/blob/main/Tian_Qin_Credit_Fraud.ipynb

The data contains customer features and a binary label where “1” indicates positive (fraud), and “0” means negative (legitimate).  

Before modeling, you will need to perform train-test split to reserve part of your data for validation. One problem of fraud detection data is that usually you will have only a few positive data points, a.k.a imbalanced dataset problem. You need to think of strategies of splitting and sampling your data to avoid the issues caused by the imbalance. 
Imbalance data could cause the following issues. Suppose we have 100 data points and only two of the mare positive: 
 - You will likely have 0 positive cases in your test data when you split randomly. 2. The model, if predicting everyone to be negative, then the accuracy would be 98%, but does it mean we have a good model?   
 
Therefore, accuracy is not the sole metric that we need to evaluate. There are precisions and recalls, AUCand F1 scores that can be considered as better metrics.   

To summarize, you will proceed the project by the following steps: 
1. Load the data and briefly explore what are the suitable columns to use as features and what is the distribution of the label. 
2. Preprocess your feature set. If your data contains significant imbalance problems, think of strategies to draw representative validation sets. Besides, think of how to re-balance your TRAINING dataset . 
3. Once you have cleaned X_train, X_test, Y_train and Y_test, start building your NN, by using keras, this is as simple as a few lines of code. 
4. Train your model with your training set. You may play with hyperparameters such as number of layers, size of hidden neurons, different activation functions, learning rate, number of epochs to improve your model performance. 
5. Evaluate your model with your reserved validation set and report your performance in accuracy, precision and recall. Discuss briefly what you observe from these metrics. 
6. [Bonus] Try if you can implement some other classic ML algorithm and compare in terms of performance and computation time. 
7. [Bonus 2] If you can learn more about and apply dropout, batch normalization and weight initialization to see if you can further improve. 
8. [Bonus 3] Implement cross validation. 
9. [Bonus 4] Evaluate using AUC: https://towardsdatascience.com/understanding-auc-roc-curve- 68b2303cc9c5 
