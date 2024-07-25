# K-Fold-Analysis
This project is an assignment of Artificial Intelligence 
It uses the MNIST 
The purpose of this program is to use and analyze K-Nearest Neighbor's performance on a given dataset—in this case, the MNIST dataset through K-Fold Cross-Validation.

The MNIST dataset is an extensive and reliable set of data is provided by this dataset, which can be used to test classification systems.
The model is trained and tested on each fold once the data is divided into 1folds, guaranteeing that the model's performance is independent of the specific train-test split. This gives a more broadly applicable measure of the accuracy of the model.

The data is split into ten parts and the model is trained and tested ten times, according to the KFold object's ten splits. Each split cntains data in which the program is trained on. Iterating over each 9 parts of training and one for testing until each part has undergone both the code to do so is:

from sklearn.model_selection import KFold
kfold=KFold(n_splits=10, random_state=11, shuffle=True)
kfold
Analysing Cross Val Score: 
The cross_val_score function divides the dataset into k folds, as indicated by kfold, in order to carry out cross-validation. The model (knn in this case) is tested on the last fold after being trained on k-1 folds for each fold. Every fold is utilized as a test set exactly once during the k iterations of this operation.
The cross_val_score function divides the dataset into k folds, as indicated by kfold, in order to carry out cross-validation. 

Accuracy of the Model
Mean accuracy: 97.255714%
