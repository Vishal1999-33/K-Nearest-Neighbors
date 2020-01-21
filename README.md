# K-Nearest Neighbors(KNN)
K- Nearest Neighbors is a

->Supervised machine learning algorithm as target variable is known.

->Non parametric as it does not make an assumption about the underlying data distribution pattern.

->Lazy algorithm as KNN does not have a training step. All data points will be used only at the time of prediction. With no training step, prediction step is costly. An eager learner algorithm eagerly learns during the training step.

->Used for both Classification and Regression.

->Uses feature similarity to predict the cluster that the new point will fall into.

# What is K is K nearest neighbors?
K is a number used to identify similar neighbors for the new data point.

Referring to our example of friend circle in our new neighborhood. We select 3 neighbors that we want to be very close friends based on common thinking or hobbies. In this case K is 3.

KNN takes K nearest neighbors to decide where the new data point with belong to. This decision is based on feature similarity.

# How do we chose the value of K?
Choice of K has a drastic impact on the results we obtain from KNN.

We can take the test set and plot the accuracy rate or F1 score against different values of K.

We see a high error rate for test set when K=1. Hence we can conclude that model overfits when k=1.
For a high value of K, we see that the F1 score starts to drop. The test set reaches a minimum error rate when k=5. This is very similar to the elbow method used in K-means.
Value of K at the elbow of test error rate gives us the optimal value of K.

