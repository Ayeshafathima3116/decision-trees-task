🌲 Task 5: Decision Trees and Random Forests
🎯 Objective
To classify heart disease presence using tree-based models — Decision Tree and Random Forest, and analyze model performance, feature importance, and overfitting control.

📘 Dataset
Filename: heart.csv

Shape: 303 rows × 14 columns

Target Variable: target (0 = No disease, 1 = Has disease)

Missing Values: ✅ None

🧰 Tools & Libraries
Language: Python

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn

📊 Workflow & Methodology
✅ Step 1: Data Preprocessing
No missing values found.

Features separated from the target.

Dataset split into training (80%) and test (20%) sets.

✅ Step 2: Decision Tree Classifier
Trained a basic Decision Tree model.

Accuracy: ~77%

Evaluation: Used confusion matrix and classification report.

Visualization: Tree plotted using plot_tree().

✅ Step 3: Controlled Overfitting
Set max_depth=4, min_samples_split=10 to prune tree.

Accuracy slightly improved: ~80–82%

✅ Step 4: Random Forest Classifier
Used 100 estimators for ensemble learning.

Accuracy: ~86%

Significantly more stable and generalizable than a single tree.

✅ Step 5: Feature Importance
Top Features:

cp (chest pain type)

thalach (max heart rate)

exang (exercise-induced angina)

✅ Step 6: Cross-Validation
5-Fold CV Mean Accuracy: ~84–86%

Confirms consistency of Random Forest performance.

📝 Results Snapshot
Model	Accuracy	Highlights
Decision Tree	~77%	Simple, interpretable
Pruned Tree	~81–82%	Reduced overfitting
Random Forest	~86%	Best performance + high stability
5-Fold CV (RF)	~84–86%	Confirms robustness

📌 Learnings & Takeaways
Decision Trees are interpretable but prone to overfitting.

Pruning improves generalization.

Random Forests outperform single trees and provide feature importances.

Cross-validation ensures model stability.

