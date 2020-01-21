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

![1_ZiHTPANDXvBHV5HmIDeQCw](https://user-images.githubusercontent.com/54469035/72787171-6a358300-3c55-11ea-9c02-15d8bcc4f904.png)

# How does KNN work?
Step 1: Choose a value for K. K should be an odd number.

Step2: Find the distance of the new point to each of the training data.

Step 3:Find the K nearest neighbors to the new data point.

Step 4: For classification, count the number of data points in each category among the k neighbors. New data point will belong to class that has the most neighbors.

# How is the distance calculated?
Distance can be calculated using:-

1)Euclidean distance:-Euclidean distance is the square root of the sum of squared distance between two points. It is also known as L2 norm.

![1_HWpWqDw1Fz5zuYkDI_C0yg](https://user-images.githubusercontent.com/54469035/72787474-019ad600-3c56-11ea-9f1b-9a417220a059.png)

2)Manhattan distance:-Manhattan distance is the sum of the absolute values of the differences between two points.

![1_4cvR49dI1ufYqUJNlls67g](https://user-images.githubusercontent.com/54469035/72787544-25f6b280-3c56-11ea-85f4-b719cf7d1aa2.png)

3)Hamming Distance:-Hamming distance is used for categorical variables. In simple terms it tells us if the two categorical variables are same or not.

![1_ZpyVp_0m21ZvmIZQnu35fQ](https://user-images.githubusercontent.com/54469035/72787638-4f174300-3c56-11ea-8a27-b744f41585e3.png)

4)Minkowski Distance:-Minkowski distance is the used to find distance similarity between two points. When p=1, it becomes Manhattan distance and when p=2, it becomes Euclidean distance.

![1_L6GE6h0gV4imp-U3S2mTrw](https://user-images.githubusercontent.com/54469035/72787725-7a9a2d80-3c56-11ea-9093-95218f3c0d2b.png)

# Principal component analysis (PCA)
Principal component analysis (PCA) is a statistical procedure that uses an orthogonal transformation to convert a set of observations of possibly correlated variables into a set of values of linearly uncorrelated variables called principal components. This transformation is defined in such a way that the first principal component has the largest possible variance, and each succeeding component in turn has the highest variance possible under the constraint that it is orthogonal to the preceding components. The resulting vectors are an uncorrelated orthogonal basis set. PCA is sensitive to the relative scaling of the original variables.
