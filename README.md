# Simple_Three_Model_Comparison_Machine_Learning_Stroke_Prediction
This is a studying project for stroke prediction by using machine learning with three model comparison (RandomForest,CatBoost,XGBoost)

# Problem Background
Stroke is a serious medical condition that can lead to severe disabilities or even death if not promptly diagnosed and treated. It is essential to identify individuals at risk of stroke to implement preventive measures and provide timely interventions. Traditional risk assessment methods rely on medical history, physical examinations, and laboratory tests, which may not always capture the full spectrum of risk factors or predict outcomes accurately.

This study aims to leverage supervised machine learning techniques to develop a predictive model for stroke risk assessment. By analyzing a diverse range of health-related attributes and lifestyle factors, we seek to enhance the accuracy and efficiency of stroke prediction. Traditional risk assessment methods often have limitations in capturing complex interactions between various risk factors, leading to suboptimal predictions.

Supervised machine learning offers a promising approach to address these limitations by automatically learning patterns and relationships from data to make predictions. By training the model on historical data of individuals with and without strokes, we can create a predictive algorithm capable of identifying patterns indicative of stroke risk.

Furthermore, the development of such a predictive model can aid healthcare professionals in early detection and intervention, potentially reducing the incidence and severity of strokes. Additionally, it can empower individuals to take proactive measures to mitigate their stroke risk through lifestyle modifications and targeted interventions.

In summary, this study aims to harness the power of supervised machine learning to improve stroke prediction, thereby contributing to more effective preventive healthcare strategies and better patient outcomes.


# Aims
The study aims to improve our knowledge and understanding of supervised machine learning algorithms for classification. We should know how supervised machine learning algorithms work to fully understand and utilize the concept and algorithms of supervised machine learning. The second objective of this study is also improving our skills in applying and improving the chosen algorithms. This is because there are many ways to improve our models' accuracy to achieve the correct prediction through our analysis. The third objective is achieving 80% accuracy, which the model selected.

# Random Forest
Random Forest Hyperparameter Tuning using GridSearchCV
The algorithm is first utilized by selecting the importance from the above test data. Then after that, we will input the data into the algorithm which then we could apply hyperparameter tuning by changing the parameters that are being fed into the algorithm such as our CV which is the number of folds for the K-cross validation and scoring which defines the performance measure of the algorithm. Then we will call the fit function which will provide all the training data and train the model using all hyperparameter combinations and perform cross-validation to evaluate their performance.
Check Accuracy on Test Data
We will then create a confusion matrix for both train data and test data to check the accuracy of said data. The Random Forest algorithm after it has been trained with the accuracy of 100% has returned a test accuracy of 93.74%

# CatBoost
Setting up the model

To set up CatBoost, we will first need to call the classifier by using CatBoostClassifier(). Then we are to provide two parameters for said function which is iterations which specifies the maximum number of trees that can be built when creating the model. Next is the learning rate which defines the rate of the model learning. After the classifier is called, we will then fit the data obtained from above and fit it into the algorithm.
Check Accuracy on Test Data
We will then create a confusion matrix for both train data and test data to check the accuracy of said data. The Gradient Boosting algorithm after it has been trained with the accuracy of 95.94% has returned a test accuracy of 93.84%

# XGBoost
Setting up XGBoost model

To utilize this code, first we need to convert our dataset into DMatrix class which in turn can optimize the speed and memory use for effective dataset processing. To use DMatrix, we will then call the DMatrix() function which requires the parameters such as the data and labels. Then we will create the model by calling the function ‘train()’ and providing a few hyper parameters such as the tree depth, learning rate and binary logistic objective. We also need to provide boosting rounds which helps train the model.
Check Accuracy on Test Data
We will then create a confusion matrix for both train data and test data to check the accuracy of said data. The XG Boost algorithm after it has been trained with the accuracy of 99.68% has returned a test accuracy of 93.95%

