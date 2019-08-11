# machine-learning-model-evaluation-iris
Performance comparion of various machine learning models on background and foreground classification for iris data.

### Dataset creation

1. 50 iris images were used to create the dataset. 
2. From each image 5 patches for foreground and background were selected having length 21X21.
3. GLCM properties were applied on each iris patch:
	- contrast
    - dissimilarity
    - homogeneity
    - energy
    - correlation
    - ASM
4. Class label 1 for foreground and class label 0 for background were assigned. 
5. Final database file 'iris.csv' having shape (500, 7) was created.
6. 'iris_pickle' file was used to read created database file, created X and y, divided them into training and testing data and standardized them using Standard Scalar.  

### Machine learning models used:
1. Logistic regression
2. Support Vector Machines - linear and rbf
3. Decision Trees
4. Random Forest
5. Adaboost classifier
6. Gradient boost classifier

### Model Selection

Except for Logistic regression, best model for each machine learning method is selected using hyperparameter tuning.

### Evaluated results for each model

1. Cross validation score
2. Mean score
3. Standard deviation
4. Confusion matrix
5. Precision, Recall and F1 score

### Performance Chart 

![alt text](https://github.com/anurooprtj/machine-learning-model-evaluation-iris/blob/master/iris.csv)

