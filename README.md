## On-Time-Flights-Arrival-Classifier

### Description
Predict on-time arrivals of airlines among top 10 busiest airports.  Flight data are obtained from Bureau of Transportation Statics http://transtats.bts.gov/Tables.asp?DB_ID=120&DB_Name=Airline%20On-Time%20Performance%20Data&DB_Short_Name=On-Time (Jan~Oct,2016)

### Model Developing Process

1. Import Data
2. Explore Data
   * Remove 'nan' and outliers
   * Simplify data set to top 10 airports only.
   * Select key features, X intuitively
3. Preprocess Data
  * Convert categorical data into binary format using "pd.get_dummies' ( =LabelEncoder + OneHotEncoder)
  * Scale Data - not needed this application 
4. Split data in train and test set
5. Appy PCA on X_train - See if you can reducec # of features
6. Try out a few classifiers on the train set
  * Decision Tree
  * Random Forest
  * SVM
  * Logistic Regression
  * GaussianNB
7. Cross-validate within train set and downselect
8. Fine tune with GridSearchCV
9. Evaluate the classifier performance on the test set (=unseen data)

### Usage
* Jupyter Ipython.
* python 2.7
