# On-Time-Flights-Arrival-Classifier

Purpose
Predict on-time arrivals of airlines among top 10 busiest airports.  Flight data are obtained from Bureau of Transportation Statics http://transtats.bts.gov/Tables.asp?DB_ID=120&DB_Name=Airline%20On-Time%20Performance%20Data&DB_Short_Name=On-Time (Jan~Oct,2016)

Model Developing Process
Import Data
Explore Data
   Remove 'nan' and outliers
   Simplify data set to top 10 airports only.
   Select key features, X intuitively
Preprocess Data
  Apply LabelEncoder
  Apply OneHotEncoder
  Scale Data - not needed this application 
Split data in train and test set
  Appy PCA on X_train
Try out a few classifiers on the train set
  Decision Tree
  Random Forest
  SVM
  Logistic Regression
  GaussianNB
Cross-validate within train set and downselect
Fine tune with GridSearchCV
Test the classifier performance on the test set (=unseen)

Usage
Jupyter Ipython.
python 2.7
