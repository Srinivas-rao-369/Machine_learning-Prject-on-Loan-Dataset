# Machine_learning-Prject-on-Loan-Dataset
It is a classification problem. And i have tested it with different models.
Loan_data_trained_model

Predict whether a loan can be provided/granted to a particular person or not and if yes predict how much? (Classification and regression)

1)	How cleaning/EDA was performed:
    We need to read the data description in order to understand what each column means.
    After understanding the data description ,find out the 
      a)	missing values , outliers , relation between independent and dependent features.
      b)	Here I used heatmap , boxplots to find out the relation and outliers.
      c)	We removed the outliers from the columns like ‘ApplicantIncome’.
      d)	We filled the missing values in the columns  like Gender', 'Married', 'Dependents','Self_Employed', 'LoanAmount', 'Loan_Amount_Term', 'Credit_History'.
      e)	While filling the missing values we did an analysis that which values can be filled in place of missing values.and 
      f)	Visualize the data using boxplots, histograms .
2)	Your independent and dependent feature

      a)	We have 12 independent variables and 1 target variable, i.e. Loan_Status in the training dataset.
      b)	Independent features: 'Gender', 'Married', 'Dependents', 'Education','Self_Employed', 'log_of_CoapplicantIncome', 'log_of_ApplicantIncome','log_of_Loan_Amount_Term',             'Credit_History', 'Property_Area','log_of_LoanAmount',  'log_of_TotalIncome'.
      c)	Dependent feature:
          'Loan_Status’

3)	Why and how selection/engineering/scaling was performed
      
      a)	Scaling modifies features to lie between a given minimum and maximum value, often between minus one and one, or so that the maximum absolute value of each feature is             scaled to unit size to improve the numerical stability of models.
      b)	We did scaling with Normalizer techniques.
          i)	We apllied normalizing on the numerical data in order to standardize the numerical data.
          ii)	We did it on 'LoanAmount','CoapplicantIncome','ApplicantIncome', 'TotalIncome' .
         iii)	Feature selection with Correlation Matrix with Heatmap and feature importance
         
4)	Encoding 

      a)	Label Encoding: Each category is given one label (e.g. 0, 1, 2 etc). Label encoding is a technique to encode categorical variables. 
      b)	We did Label encoding on ‘cat_cols’.
      
5)	Model and Ensembling:
      
      a) Model:
          i)	Naive Bayes
          ii)	KNeighborsClassifier
          iii)	Logistic Regression

               Model                       Accuracy(%)
            Naive Bayes	                0.8211382113821138
         KNeighborsClassifier	          0.8130081300813008
          Logistic Regression	          0.8373983739837398



    b)	Ensembling:
          i)	VotingClassifier :
            
                Model 	            Accuracy(%)
      RandomForestClassifier	    0.8211382113821138

 

     

  







