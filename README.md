# Titanic_Survivor_Prediction

This was one of my first project wehn I set my foot in the Machine Learning Domain, 

Information regarding the Dataset:

Data Dictionary: 

survival	- Survival	0 = No, 1 = Yes
pclass	- Ticket class	1 = 1st, 2 = 2nd, 3 = 3rd
sex	- Sex	
Age	- Age in years	
sibsp	- Number of siblings / spouses aboard the Titanic	
parch	- Number of parents / children aboard the Titanic	
ticket -	Ticket number	
fare -Passenger fare	
cabin	- Cabin number	
embarked	- Port of Embarkation	C = Cherbourg, Q = Queenstown, S = Southampton

pclass: A proxy for socio-economic status (SES)
1st = Upper
2nd = Middle
3rd = Lower

age: Age is fractional if less than 1. If the age is estimated, is it in the form of xx.5

sibsp: The dataset defines family relations in this way...
Sibling = brother, sister, stepbrother, stepsister
Spouse = husband, wife (mistresses and fiancés were ignored)

parch: The dataset defines family relations in this way...
Parent = mother, father
Child = daughter, son, stepdaughter, stepson
Some children travelled only with a nanny, therefore parch=0 for them

Steps for Execution:

1. Extracted the Data inta a DataFrame.
2. Perfromed EDA for the different features to check how they ar correlated.
3. Imputed the missing values and dropped 'Cabin  column for the missing values which can't be imputed, because a major chunk of missing values were missing from the feature.
4. Performed One Hot Encoding for the categorical features ' Pclass', 'Sex','Embarked',Ticket'.
5. Dropped the irrelevent features which won't be used anymore.
6. As the data give was separate for the train set an test set, assigned the proper features for X and y.
7. Created a Machine Learning Model using Logostic Regression earlier and then followed by scaling the values using MinMaxScaler.
8. Created a seomodel with RandomForestClassifier Algorithm using n_estimators=600 just to check howRandom Forest Classifier performed as compared to Logistic Regressor.  
9. Exported the results to the csv file.
