# Machine-Learning-for-Real-Estate-Price-Prediction
# Meijuan Hu
![ML house price](https://github.com/qiluchuan/Machine-Learning-for-Real-Estate-Price-Prediction/assets/160643225/22c6a381-c9de-4fe7-aa1d-559383d10fe8)


# Description
This project is to replicate and extend the findings from the article “The Use of Machine Learning in Real Estate Research” by implementing various machine learning and deep learning models. The machine learning techniques Kernel Ridge Regression (KRR), Support Vector Regression (SVR), and Deep Neural Networks (DNN) are performed
# Proposed Method
## Data collection and preprocessing
Prior to modeling, summary statistics and a histogram of Residential Property Prices (RP) were
created to visualize the data. The summary statistics show the mean is of RP is 4.06 and the median
is 3.59 which indicate the data are skewed (skewed to the right) and there are some extreme values
(outliers) in the dataset. Very high or low values can pull the mean in the direction of outlier, causing
a large difference between the mean and median. 
## Model implementation
Transformation is used for this dataset since the distributions before scaling are not normally distributed. The distributions after standard scaling is more comparable, and the features ‘GFA’, ‘AGE’,
and ‘ZZ’ show bimodal shapes. The distribution of all features are skewed to the right. The standardized features are used to build the models. The implementation of KRR model, SVR model, and
DNN using ‘sklearn.kernel_ridge’, ‘sklearn.svm’, and ‘keras’ in Python, respectively
 ## Model Performance Comparison
- The model evaluation is used for this section. The Mean Squared Error (MSE), Root Mean Squared
Error (RMSE), Mean Absolute Error (MAE), R2
, and Mean Absolute Percentage Error (MAPE)
are commonly used to evaluate the performance of regression models. MSE measures the average
squared difference between actual and predicted values. RMSE represents the squared root of the
MSE, providing a measure of the average magnitude of errors. MAE measures the average absolute
difference between actual and predicted values. R2
represents the proportion of the variance in the
dependent variable that is predictable from the independent variables. MAPE measures the average
percentage difference between actual and predicted values, normalized by actual values. MAE is less
sensitive to outliers compared to MSE and RMSE since it considers the absolute difference.
- A lower MSE, RMSE, MAE, and lower MAPE generally indicates better model performance, as
it signifies that the model’s predictions are closer to the true values. The higher coefficient of
determination (R2
) generally indicates a better-fitting model.
# Discussion
- Deep Neural Networks (DNN) is suitable for this task. The architecture of the DNN, including
the number of layers, types of layers, and connectivity patterns, can influence its ability to capture
complex patterns in the data and it particularly powerful in tasks that involve complex patterns or
representation. In addition, DNN has the highest R2 value, and the lowest MSE, MAE, and RMSE.
Table 7 presents results associated with Extra Trees (ET), k–Nearest Neighbors (KNN), Random
Forest, Ordinary Least Squares (OLS), Kernel Ridge Regression (KRR), Support Vector Regression
(SVR), and Deep Neural Networks (DNN). Comparing all seven metrics with those of the ET, KNN,
Random Forest, OLS, KRR, SVR, and DNN, the Random Forest model from research paper appears
to perform well and has the highest R2 value and the lowest MSE, RMSE, and MAPE values,
indicating strong explanatory power.
![image](https://github.com/qiluchuan/Machine-Learning-for-Real-Estate-Price-Prediction/assets/160643225/9e2efb0b-6a40-4cd1-a2bc-bbbdc7f3f4f2)
