# Task-6
Task 6  AL &amp; ML Internship By Elevate Labs

Dataset : iris
Tools, pandas,sklearn, matplotlib

1. Choose a classification dataset and normalize features
We selected the Iris dataset, a classic multiclass classification dataset with three flower species.
To enable 2D visualization, we used only the first two features: sepal length and sepal width.
Although normalization wasn't essential due to similar feature scales, it can further improve KNN for datasets with varying ranges.

2. Use KNeighborsClassifier from sklearn
We used KNeighborsClassifier from sklearn.neighbors to build a KNN model.
The model was trained using the training subset of the Iris data.
This classifier assigns class labels based on the majority vote of the k nearest neighbors.

3. Experiment with different values of K
We experimented with k = 5, k = 7, and k = 9 by changing the n_neighbors parameter.
The model was retrained and evaluated each time to observe performance differences.
This helps understand the effect of underfitting (large k) and overfitting (small k).

4. Evaluate model using accuracy and confusion matrix
For each k, we computed the accuracy score and displayed the confusion matrix using ConfusionMatrixDisplay.
These metrics revealed how well the model predicted each class and overall performance.
Accuracy improved slightly as we adjusted the number of neighbors.

5. Visualize decision boundaries
We plotted decision boundaries using the first two features to visually understand class separation.
A mesh grid was created and classified using the trained KNN model to highlight boundaries.
Training and test points were overlaid to show model behavior and decision regions.
