 Task 7: Support Vector Machines (SVM)

This task is part of the **AI & ML Internship** under the Ministry of MSME. The objective of this task is to understand and implement Support Vector Machines (SVM) using both linear and non-linear kernels for classification problems.


 Objective

- Use **SVMs** for **binary classification**.
- Explore both **Linear** and **RBF (Radial Basis Function)** kernels.
- Tune hyperparameters (**C**, **gamma**).
- Visualize **decision boundaries** in 2D.
- Use **cross-validation** to evaluate model performance.

Dataset

- **Dataset**: Breast Cancer Wisconsin Diagnostic Dataset
- **Source**: Loaded directly from `sklearn.datasets`
- **Classes**: 
  - `0`: Benign
  - `1`: Malignant
- **Features Used for Visualization**:
  - `mean radius`
  - `mean texture`

 Tools & Libraries Used

- Python 3.x
- `scikit-learn`
- `NumPy`
- `Pandas`
- `Matplotlib`

 Steps Implemented

1. Loaded the breast cancer dataset from `sklearn`.
2. Selected 2 features (`mean radius`, `mean texture`) for 2D decision boundary visualization.
3. Standardized features using `StandardScaler`.
4. Split the dataset into train and test sets.
5. Trained two SVM models:
   - **Linear Kernel**
   - **RBF Kernel**
6. Tuned RBF SVM using **GridSearchCV** (for `C` and `gamma`).
7. Evaluated models using **accuracy**, **cross-validation**, and **classification report**.
8. Visualized decision boundaries using `matplotlib`.

 Evaluation Results

| Model         | Accuracy (Test Data) |
|---------------|----------------------|
| Linear SVM    | ~90%                 |
| RBF SVM       | ~91%                 |

- Best Parameters (RBF): `C = 1`, `gamma = 0.1`
- Cross-validation Score: ~89.9%

Visual Output

Two plots are generated:
1. Decision Boundary - Linear SVM
2. Decision Boundary - Tuned RBF SVM

These plots show how each classifier separates the two classes visually based on the selected features.
