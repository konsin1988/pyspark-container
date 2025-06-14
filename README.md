# Classification model competition

### Our goals are:
- Choose best hyperparameters for each of the model. To solve this problem we will use cross-validation;
- Compare three models for their ability to classify bad customers;
- Log all this manipulations to mlflow to have the opportunity to compare multiple metrics and to use best of these to the production

### Basic tools
- pyspark in jupyter notebook container - the opportunity to work with Big Data without rewritting the code;
- mlflow - logging all the parameters, metrics and models due to experiments;
- minio - s3 storage to store artifacts and models;

### LinearSVC 
This binary classifier optimizes the Hinge Loss using the OWLQN optimizer. Only supports L2 regularization currently.
##### Hyperparameters we will use in crossvalidation:
- maxIter;
- tol;
- regParam.

### Gradient Boosted Trees Classifier (GBTClassifier)
It is a technique of producing an additive predictive model by combining various weak predictors, typically Decision Trees.

##### Hyperparameters we will use in crossvalidation:
- maxDepth;
- maxIter;
- validationTol.

### Logistic Regression
Logistic regression is a supervised learning algorithm that makes use of logistic functions to predict the probability of a binary outcome.

##### Hyperparameters we will use in crossvalidation:
- maxIter;
- regParam;
- aggregationDepth.