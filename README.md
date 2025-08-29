🌸 Iris Flower Classification
📝 Overview

This project uses the Iris dataset to classify flowers into three species:
Iris-setosa, Iris-versicolor, and Iris-virginica.
It demonstrates an end-to-end machine learning workflow, including:
data exploration, preprocessing, model training, evaluation, and visualization.

📊 Dataset

Source: Kaggle CSV (https://www.kaggle.com/datasets/saurabh00007/iriscsv)


Features:

🌿 SepalLengthCm

🌿 SepalWidthCm

🌸 PetalLengthCm

🌸 PetalWidthCm

Target: Species (encoded as numeric labels: Iris-setosa=0, Iris-versicolor=1, Iris-virginica=2)

🚀 Steps
1️⃣ Data Exploration

🔍 Checked dataset info, missing values, and duplicates

🥧 Visualized class distribution with a pie chart

📊 Explored feature distributions using histograms and boxplots

🔗 Created correlation heatmap to understand relationships between features

🌺 Analyzed feature distributions per species using boxplots

💡 Observed that petal length and width are more discriminative than sepal features

2️⃣ Data Preprocessing

🗑️ Dropped irrelevant Id column

🔢 Encoded target Species to numeric values (0,1,2)

📈 Split dataset into training (60%) and testing (40%) sets with stratification to preserve class distribution

⚙️ Standardized features using StandardScaler (important for KNN, helpful for Logistic Regression)

3️⃣ Model Training

Logistic Regression

⚡ Default solver with max_iter=200 to ensure convergence

K-Nearest Neighbors (KNN)

🔹 Used k=6 neighbors (chosen empirically)

4️⃣ Model Evaluation

✅ Evaluated accuracy, precision, recall, and F1-score on the test set

📈 Visualized confusion matrices for both models

🔄 Performed 5-fold cross-validation for more reliable accuracy estimates

⚠️ Observed that misclassifications occur mainly between versicolor and virginica, which is expected due to overlapping feature values

🌟 Both models perform very well on the Iris dataset

🔄 Cross-validation shows slight variability between folds, providing a realistic evaluation

🌸 Petal features (length & width) are most important for accurate classification

6️⃣ Confusion Matrix Insights

✅ Logistic Regression and KNN perfectly classify Setosa

⚠️ Minor errors occur between Versicolor and Virginica

🔬 This aligns with the biological similarity of these two species in some feature ranges

7️⃣ Visualizations

🥧 Pie chart of class distribution

📊 Feature histograms and boxplots

🔗 Correlation heatmap

🌺 Boxplots of features by species

🧮 Confusion matrices for both models

📈 Optional: Cross-validation fold accuracy plot

8️⃣ Conclusion

💡 Logistic Regression and KNN are both highly effective for the Iris dataset

🧹 Proper preprocessing (dropping irrelevant columns, encoding, scaling) is crucial

🔄 Cross-validation provides a more realistic measure of model performance than a single train/test split

🌸 Petal features are the most discriminative, explaining the high accuracy

🎓 This project demonstrates a complete machine learning workflow, suitable for educational and reporting purposes

📎 Kaggle Notebook

You can view and run the full notebook here: https://www.kaggle.com/code/basmammdouh/iris-flower-classification ✅