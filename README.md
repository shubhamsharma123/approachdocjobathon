# approachdocjobathon

I had divided the overall problem statement into five parts
1)	Data Exploration and EDA
2)	Data Cleaning and feature engineering
3)	ML model selection & development
4)	Model Validation
5)	Prediction for test data
6)	Deploy model using flask and docker(Not asked so TBD on demand)

Observation:
1)	Data Exploration and EDA:

•	There are total 10 columns into the training data set
•	Most of the user has engagement score between 3 to 5 in train data
•	Most of the users of our video website is in the age range of 15 to 40
 

2)	Data Cleaning and feature engineering

Null values checking : 
•	There are no null values in training or testing data set

feature engineering:
•	I had converted 'gender','profession'  into categorical type
•	I had dropped 'row_id','engagement_score' from training data(X)
•	I had dropped target variable 'engagement_score' from validation data(Y)
•	I had splitted the data in 70:30 ratio of train to validation data

3)	ML model selection & development

Target variable “'engagement_score'” is numerical . So I had  to explored all the regression analysis techniques.

I had explored/implemented,
1.	Linear Regression
2.	Robust Regression
3.	Ridge Regression
4.	LASSO Regression
5.	Elastic Net
6.	Polynomial Regression
7.	Stochastic Gradient Descent
8.	Artificial Neaural Networks
9.	Random Forest Regressor

4)	Model Validation

Among all of above techniques “Random Forest Regressor
“ was the best because its r2square was hightest .
So I had used that only.
To reach till my final model I had employed 10 different algorithm which I listed in point-3 then  again I had tuned “Random Forest Regressor” by (n_estimators,min_samples_split,max_depth, random_state)
As well as I had worked on ANN also a lot . I had trained it on 240 epoches(In progressive manner from 10..50..100..140..190..240) but still ANN accuracy was less .

My model structure and how it looks is below:

 


5)	Prediction for test data
Test data were there in “test_1zqHu22” file.
I had dropped “row_id” from it and predicted 'engagement_score' using different models .
Then I uploaded on Jobathon portal and it gave me “0.2252260886” score

 


6)	Deploy model using flask and docker(Not asked so TBD on demand)
In future for deployment I can create flask-api and deploy it on docker if any company will want





