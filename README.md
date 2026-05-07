# Income-Classifier-
This project builds a machine learning model to predict whether an individual earns more than \$50K per year based on demographic and work-related features.

## 📊 Dataset
- Adult Income Dataset
- Contains demographic, education, and employment details
- Target variable: `income` (<=50K, >50K)

## ⚙️ Steps Performed

### 1. Data Cleaning
- Removed unnecessary columns: `fnlwgt`, `education`, `race`
- Handled missing values (`?`)
- Stripped extra spaces from categorical values

### 2. Feature Engineering
- Separated target variable before encoding
- Encoded categorical features using factorization

### 3. Handling Class Imbalance
- Applied **downsampling** to balance majority and minority classes

### 4. Data Splitting
- Split data into training and testing sets

### 5. Feature Scaling
- Applied **StandardScaler** on training data
- Transformed test data using same scaler

### 6. Model Training
- Used **Logistic Regression**
- Solver: `liblinear`
- Max iterations: 2000

### 7. Evaluation
- Accuracy: ~76%
- Evaluated using confusion matrix and classification report


## 📈 Results

Confusion Matrix:
[[1140 368]
[ 356 1140]]

Balanced precision and recall across classes
- Improved minority class performance after handling imbalance

## 🧠 Key Learnings
- Accuracy alone can be misleading in imbalanced datasets
- Handling class imbalance improves model fairness
- Proper preprocessing significantly impacts model performance

---

## 🛠️ Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn

---

## 📌 Conclusion
This project demonstrates a complete machine learning pipeline including preprocessing, balancing, scaling, and evaluation, with a focus on improving performance for imbalanced data.
