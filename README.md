Enhanced KNN Classification - Iris Dataset

This repository hosts a modular Python implementation of the K-Nearest Neighbors (KNN) algorithm applied to the Iris dataset. Designed to demonstrate production-level best practices, it bridges the gap between theory and practice by incorporating robust preprocessing, scientific hyperparameter tuning, and advanced visualization.

🚀 Key Features

Robust Preprocessing:
Utilizes StandardScaler to normalize feature vectors. In distance-based algorithms like KNN, unscaled features with large ranges can bias results. Scaling ensures all features contribute equally to Euclidean distance calculations, improving accuracy.

Dual-Strategy Hyperparameter Tuning:

Elbow Method: Visualizes Error Rate vs. K-value to manually identify the "elbow point"—the optimal balance between pattern capture and overfitting.

Automated GridSearch: Uses GridSearchCV to rigorously test combinations of n_neighbors and distance weights (uniform vs. distance-weighted), ensuring the mathematically optimal configuration.

Insightful Visualizations:

Pairplot: Pre-training visualization of feature correlations.

Decision Boundaries: A 2D contour plot (Petal Length vs. Width) showing how the model partitions feature space.

Confusion Matrix: A color-coded heatmap to identify specific misclassifications.

Modular Architecture:
Refactored into distinct functions (e.g., load_and_explore_data, find_optimal_k) for high readability and reusability.

🛠️ Dependencies

Ensure your Python 3.x environment includes:

pandas (Data manipulation)

numpy (Numerical operations)

matplotlib & seaborn (Visualization)

scikit-learn (Machine learning)


▶️ Usage

Run the main script to execute the pipeline:

python knn_iris_enhanced.py


📊 Results

The script outputs the optimal k value and a detailed classification report (Precision, Recall, F1-Score). It also launches interactive windows for the Elbow Curve, Confusion Matrix, and Decision Boundaries, providing a complete visual audit of model performance.
