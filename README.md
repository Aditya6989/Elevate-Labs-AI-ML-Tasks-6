🌸 Iris Classification with K-Nearest Neighbors (KNN)
📁 Project Overview
This project demonstrates the use of the K-Nearest Neighbors (KNN) algorithm to classify flowers in the Iris dataset based on petal and sepal measurements. It includes feature normalization, experimenting with different values of K, evaluating accuracy, and visualizing decision boundaries.

📊 Dataset
File: Iris.csv
Features Used:

PetalLengthCm

PetalWidthCm
(Only these two are used for 2D visualization)
Target: Species (Iris-setosa, Iris-versicolor, Iris-virginica)

✅ Steps Performed
1. Normalize Features
Standardized the input features using StandardScaler to ensure fair distance comparisons.

2. Apply KNN
Used KNeighborsClassifier from sklearn to build classification models.

3. Experiment with K
Tested different values of K (1, 3, 5, 7) to observe their effect on performance.

4. Evaluate Model
Measured accuracy and plotted confusion matrices to compare performance across K values.

5. Visualize Decision Boundaries
Visualized how the classifier separates flower species in a 2D feature space.

📦 Requirements
Python 3.x

pandas, numpy

matplotlib, seaborn

scikit-learn

Install requirements using:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn scikit-learn
📈 Results
K	Accuracy
1	~96%
3	~96%
5	~96%
7	~94%

Confusion matrices and decision boundaries show how performance and classification zones change with different K values.

🔍 Key Concepts
KNN Algorithm

Feature Scaling/Normalization

Distance Metrics (Euclidean)

Model Evaluation (Accuracy, Confusion Matrix)

Decision Boundary Visualization

📚 Learning Points
Choosing the right K affects bias-variance tradeoff

Normalization is critical for distance-based algorithms

KNN is intuitive but can be computationally expensive on large datasets

Decision boundaries can help explain model behavior visually

