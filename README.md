# Credit-Score-Classification

# Description of the Competition
## Business Scenario. 
Welcome to the high-stakes world of Global Finance Inc., where you have as- sumed the role of the lead data scientist. Your company, with its vast expanse of banking and financial services, has amassed a considerable amount of data, ranging from basic banking details to intricate credit histories of clients who span the globe.
## Business Challenge. 
The top brass (your management) has laid down a strategic initiative: to stream- line the credit assessment process. They envisage an automated system that can swiftly and accurately categorize clients into distinct credit score brackets, thereby enhancing the efficiency of the credit eval- uation process and enabling more informed decision-making.

## Your Objective. 
Your task is to develop a sophisticated machine-learning model that leverages the wealth of credit-related information at your disposal to classify clients into appropriate credit score brackets. This system should serve as a robust analytical tool that aids in the accurate assessment of credit risks and the allocation of credit scores.
Get ready to dive into the data, draw insights, and deploy your model—the future of credit scoring at Global Finance Inc. rests in your capable hands. Let the challenge commence!


## Kaggle website. 
The website to access the Kaggle challenge is the following: https://www.kaggle.com/t/455e5a7439604231a46c3a405f0a6035
In this website, you will find the dataset as well as an example notebook (sample submission.ipynb under the Discussion link) that will help you to structure your code.


# Summary of the Pipeline
The pipeline that will be followed in the project is similar to the one followed in the labs. Next we briefly describe each part of the pipeline. The pipeline is contained in the sample submission.ipynb python notebook, which also provides a simple baseline model.
• Featureengineeringanddimensionalityreduction:Thenextstepinvolvesthefeatureengineeringtask, i.e., how to select a subset of the features that will be used in the learning task (feature selection) or how to create new features from the already existing ones (see also previous section). Moreover, it is possible to apply dimensionality reduction techniques in order to improve the performance of the algorithms.
• Learning algorithm: The next step of the pipeline involves the selection of the appropriate learning (i.e., classification) algorithm for the problem. Here, you can test the performance of different al- gorithms and choose the best one (e.g., logistic regression, SVMs, decision trees, neural networks). Additionally, you can follow an ensemble learning approach, combining many classification al- gorithms. You are not restricted to use only the models covered in the course but rather using any ML model offerered in scikit-learn (https://scikit-learn.org/stable/index.html) or in similar libraries.
• Evaluation: In the next section, we describe in detail how the evaluating will be performed. Keep in mind that the challenge corresponds to a multi-class classification task.
# Evaluation
You will build your classification model based on the training data contained in the train set.csv file. To do this, you can apply cross-validation techniques1. Of course, having a good model that achieves good accuracy under cross validation does not guarantee that the same accuracy will also be achieved for the test data. Thus, the final evaluation of your model, will be done on the test dataset contained in the test set.csv file. After having a model that performs well under cross-validation, you should train the model using the whole training dataset (i.e., all the instances of the train set.csv file) and test it on the test dataset as described below.
## How to evaluate your model on the test dataset?
For the test data (test set.csv) we do not have information about the class labels (type of each email), and thus the final assessment will be done in the Kaggle platform. Note that, the same prepro- cessing tasks that have been applied on the training data should also be applied on the test data. The evaluation process can be summarized as follows:
1. Run your model on the test data (test set.csv).
2. Get the predicted class labels for each instance of the test dataset.
3. Create a new file, called sandbox submission.csv, that contains the predicted class label for each instance. The pipeline is given in the example notebook (sample submission.ipynb).
4. Create an account on Kaggle (the same for each member of your team) and make a new sub- mission by simply uploading the sandbox submission.csv. Then, Kaggle will evaluate your predictions, and the evaluation score as well as your position (with respect to the rest users) will appear in the Leaderboard. Note that, you can submit up to 10 entries per day. Your final score will be the best one that you have achieved.

# Grading
Grading will be on 100 points total. Each team should deliver:
• A submission on the Kaggle competition webpage. 40 points will be allocated based on raw performance only, provided that the results are reproducible. That is, using only your code and the data provided on the competition page, we should be able to train your final model and use it to generate the predictions you submitted for scoring.
• A 3-pages report (see details below). Please ensure that both your real names and the name of your Kaggle team appear on the report.
The 3-page report should include the following sections (in this specific order):
• Section 1: Feature engineering [25 points]. Regardless of the performance achieved, we will re- ward the research efforts and creativity put into the feature engineering step (e.g., creation of new features). You are expected to:
1. Explain the motivation and intuition behind each feature. How did you come up with new feature? What is it intended to capture? Did you discard other features?
2. Rigorously report your experiments about the impact of various combinations of features on predictive performance, and, depending on the classifier, how you tackled the task of feature selection.
• Section 2: Model tuning and comparison [25 points]. You are expected to:
1. Comparemultipleclassifiers(e.g.,SVMs,RandomForest,Boosting,Logisticregression,Near-
est neighbors).
2. For each classifier, explain the procedure that was followed to tackle parameter tuning and prevent overfitting.
3. Report the cross-validated performance (on the training data) of the models you have ex- plored, as well as the score on the test set (given by Kaggle).
4. Discuss about any additional models that you have tested but did not perform well.
Report and code completeness, organization and readability will be worth 10 points. Best submis- sions will (i) clearly deliver the solution, providing detailed explanations of each step, and (ii) provide clear, well organized and commented code.

# How to Submit
Please complete the second assignment in groups of 3-4 students (preferably, the same team as in the
project of the course). No late assignments will be accepted.
1. Kaggle submission: submission of your solution in the kaggle platform (team submission – pick also a name for your team).
2. Report: typeset your report (PDF file only). In your report, you should mention the name of your team in Kaggle, and the names of all team members. The submission of the report (max 3 pages) should be made on gradescope (Kaggle Challenge). Only one member of each teams needs to do the submission, adding the rest as team members.
3. Code: prepare a .zip file (code name of your team.zip) containing the code that is needed to reproduce your submission. The file should be sent by email to: centralesupelec.fmlclass@gmail.com. The subject of the email should be: “[DSBA-FML] - Assignment 2 Code - Name of Your Team”.
