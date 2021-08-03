# 21-machine-learning-challenge
This assignment had three requirements:

  *Preprocess a dataset to be used with Machine Learning 
  Step 1:  Preprocess the dataset prior to fitting it to the selected model
  Step 2:  Perform feature selection on remove unnecesary features
  Step 3:  Use MinMaxScaler to scale the numerical data
  
  *Tune the Machine Learning model parameters
  Step 1:  Use GridSearch to turn model parameters
  Step 2:  Tune and compare at least two different classifiers
  
  *Report the Results
  Step 1: Compare the performance of the models 
  Step 2: Summarize findings
  Step 3: Identify the models that show the best scoring in accuracy of prediction of the existence of exoplanets

Four machine learning classification models were considered.  They were:  Logistic Regression, SVM, Nearest Neighbor, and Random Forest.  Best performing classifier was the Random Forest model that used the ExtraTreeClassifier for feature selection, see Final_RF.IPYNB.  The next best performing classifier was the Nearest Neighbor - Final_KNN_Feature.IPYNB that used GradientBooster for feature selection.  It was also noted that when the feature selection used for Logistic Regression, was GradientBooster the accuracy of prediction went up to 88%, see Final_LogisticRegression_FeaturesChanged.IPYNB. The SVM classifier was set up slightly differently from the other classifiers, to see if comparing a poly kernel to a rbf kernel would show more accurate results.  It is interesting to note that changing the way feature selection was made, had a greater effect in changing prediction accuracy +2% - see Final_SVM_ChgKernel.IPYNB and Final_SVM_ChgKernelChgFeatures.IPYNB.

It would take more testing to see if the predictions and false positive results are truly stable, but most of the models showed the results that were between 85% and 88% which suggests that the data set was general enough and the models were not overtrained.

The most reliable classifier would be a GaussianClassifier, and it would be interested to use it with a SVM model to see what the results would be to compare the accuracy of the models used in this assignment.



