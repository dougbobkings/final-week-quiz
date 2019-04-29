# Data Science Quiz

### Instructions

- Fork and Clone
- Work on quiz
- Push back up to your repository

### Questions

1. A vector is given, `[2,3,9]`. What's the norm?
9.7

2. I have a biased 6-sided die. P(T) = 0.45. What's the probability, if I flip the coin 100 times, that I will get exactly 14 heads?

If it was a biased coin (not a die). 

2.89 ^ 11

3. What is the rank of a matrix?

The maximum number of linearly independent vectors in a matrix 


4. Why is rank important for Linear Regression?

In order for Linear Regression to function properly the columns and rows of data should be linearly independent. The colinearity of the columns will mess up the model because one column could be used to predict the other column.

5. What is the purpose of the sigmoid function in a Logistic Regression model?

It turns lod odds into probabilities.  If you specify the threshold it will help you classify the predictions.

6. What is bias vs variance?
Bias is the difference between the average prediction of our model and the correct value which we are trying to predict.
Variance is the variability of model prediction for a given data point or a value which tells us spread of our data. It measures how far the dataset is from the mean.


7. What is a hyperparameter? What part of the dataset (train, validation or test) is responsible for determining this value?
A hyperparameter is a setting of the model that is determined before the model begins to learn. If we're using a grid search, the hyperparameters are determined using the validation data set.


8. Model selection via cross validation. What part of the dataset (train, validation or test) is responsible for choosing the best model?
The validation part of the dataset is responsible for choosing the best model.

9. What is parametric vs non-parametric model?
Parametric models are numerical based (assumes a distribution to the dataset) vs non-parametric models which are based on non-numerical models (no assumptions that they fit to any distribution).

10. What models do you need to scale the data prior to fitting?
Any models that use Euclidean distances - most of the time, datasets will contain features highly varying in magnitudes, units and range

11. What is entropy? Which model uses this concept?
The measure of disorder in data in decision trees (random forests as well).  It uses it to decide on how to split.  


12. How is a random forest generated?
A random forest is a collection of decision trees that are split on different features. When the forest makes a prediction it will either take the average or the majority depending on if the model is a regression or classification. This method reduces variance.

13. How do you determine the correct number of clusters when using KMeans?
There are different methods to help determine the correct number of clusters if it is not being set by the user (e.g. there were 3 classes of wine or the user knows how many groups they want). 

Essentially, the methods (elbow, average silhouette) fit the model varying the number clusters. 

The elbow method scores each algorithm (varying k) using within-cluster sum of squares and the user looks for a bend in the graph.  The larger the better

The average silhouette method scores each algorithm using the average silhouette and the user looks for the highest average silhouette value.

14. What is a dendrogram?
A dendrogram is a visual representation of hierarchical clustering that shows how the data points are clustered together.

15. What is linkage?
Linkage is the distance between clusters. Simple, Complete, Average, and Centroid Methods are the main versions.

16. How does a recommender model work?
Recommender models look at user items and how they interact. Basically similarity of users and items.

17. How can you reduce the number of features in a model?
Lasso, PCA, feature importance, or correlation to name a few

18. What is a good use of PCA?
PCA is best used for visualization, data clustering, and datacompression.

19. In general, how do neural networks "learn"?
Neural networks learn through a process called back propagation. Data is fed through the layers of a network, an output is produced, some type of error calculation is done and the error is fed back to the network. This process continues until the error is kept at a minimum.

20. What is your favorite model? Why?
Random Forest. I believe it is easier to understand how the model is working and how flexible it is when changing how the model works. Also, when making comparisons to other models in class, it seems to give me better scores (based on the different scoring methods at the time).