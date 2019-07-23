# Marketing Data Analysis of a Bank (Machine Learning) 

An assignment project which analyzes the demographic and marketing campaign related information of client records to predict if he/she will subscribe to the product or not.

### 1-Exploratory Data Analysis

##### - For Numerical Columns
1- Analysis of each Numerical variable by plotting Boxplot with respect to target variable. 
2- Some Independent numerical variable ('balance', 'duration', 'campaign', 'pdays', 'previous') contains many outliers.  
3- I choose a range based on Maximum and Minimum value for each Numerical variable by observing Boxplot of corresponding variable. Any value out of this range will be treated as Outlier and same will be imputed by Mean of corresponding variable

##### - For Categorical Columns
1- Analysis of each Categorical variable by plotting Crosstab with respect to target variable. 
2- If any Categorical variable has more than 50% ‘unknown’ values('poutcome') or seems highly unbalanced ('default') or seems having negligible impact on target variable (‘contact’), we can drop that variable from dataset. 
3- Variables having less than 50% ‘unknown’ values are imputed by Mode of respective variable. 


### Feature Engineering
1- Created new dummy variables to convert Categorical into Numerical. 
2- Total variables after creating dummies becomes 39. 

### 2-Feature Selection
1- Feature selection by Principal Component Analysis. 
2- I have selected first 32 components out of 39

### 3-Model Training
##### Implement the following along with Cross Validation:
- Logistic Regression
- Linear Discriminant Analysis
- K-Nearest Neighbor
- Decision Tree
- Naive Bayes
- Support Vector Machine 

### 4-Model Selection
- ```Support Vector Machine``` has highest Accuracy (89.35%) but it is taking more time compare to other algorithms. 
- ```Logistic Regression``` also has nearly same accuracy (89.17%) and it is very faster than SVM. 
3. So I have considered Logistic Regression as Best model for prediction. 

### 5-Prediction
Prediction on Validation Dataset by Logistic Regression with following result: 
- Accuracy – 0.88            
- F1-score – 0.87 

### 6-Source File
[Source File](cls_model.ipynb)
