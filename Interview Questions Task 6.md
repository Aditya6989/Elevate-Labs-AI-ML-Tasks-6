1. How does the KNN algorithm work?
K-Nearest Neighbors (KNN) is super simple—it looks at the K closest points to a new data point and lets them "vote" on the label. 
For example, if most of your 5 closest neighbors are labeled "Iris-setosa", KNN predicts the new point is also "Iris-setosa".

2. How do you choose the right K?
Choosing K is all about balance.
A small K (like 1) makes the model sensitive to noise and overfitting.
A large K smooths things out but might overlook local patterns.

3. Why is normalization important in KNN?
KNN relies on distance, so if one feature (like height in cm) has values way larger than another (like weight in kg), it can dominate the distance calculation. Normalizing scales all features so they contribute equally.

4. What’s the time complexity of KNN?
KNN has no training phase, but at prediction time, it compares the test point to every training point—so prediction is slow.
Time complexity: O(n × d) per prediction (n = training samples, d = features).

5. What are the pros and cons of KNN?
Pros:
Simple and intuitive
No training time
Works well for small datasets

Cons:
Slow for large datasets
Sensitive to irrelevant or redundant features
Needs proper scaling
Doesn’t perform well in high dimensions (curse of dimensionality)

6. Is KNN sensitive to noise?
Yes! Very much. Since it bases decisions on local neighbors, just a few noisy data points can lead to wrong predictions—especially with low K values.

7. How does KNN handle multi-class problems?
No problem—KNN handles multi-class tasks naturally. 
It just counts the votes from the nearest neighbors and picks the class that appears most often, whether there are 2 or 10 classes.

8. What’s the role of distance metrics in KNN?
KNN needs a way to measure “closeness.” That’s where distance metrics come in:
Euclidean is most common (straight-line distance)
Others include Manhattan, Minkowski, and cosine
Different metrics can lead to very different results, especially if your data has unusual shapes or outliers.