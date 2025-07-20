# wine-ml-regression

#  Wine Quality Regression Model

This project demonstrates how to build and evaluate a **regression model** using Scikit-Learn to predict wine quality based on physicochemical attributes. 
The model achieves strong performance with an **R² Score of 0.9055**, indicating excellent prediction accuracy.


##  Objective

The goal of this project is to:
- Apply supervised learning techniques for regression
- Train and evaluate a model to predict wine class
- Use key evaluation metrics such as **MSE**, **RMSE**, and **R²**
- Visualize prediction performance using plots


##  Dataset

- **Source:** Wine dataset from `sklearn.datasets.load_wine()`
- **Features:** 13 numerical attributes like alcohol, magnesium, flavanoids, etc.
- **Target:** Wine class (converted to continuous regression target for demonstration)


##  Technologies Used

- Python
- Scikit-Learn
- Pandas
- NumPy
- Matplotlib
- Seaborn


##  Model Building

### 1. Load & Split Data

```python
from sklearn.datasets import load_wine
from sklearn.model_selection import train_test_split

data = load_wine(as_frame=True)
X=df.drop("target",axis=1)
y=df["target"]

X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)
```
### Output 
1.   <img width="1004" height="707" alt="Image" src="https://github.com/user-attachments/assets/18d4647e-6356-40ae-8ce5-99b79ebb07e5" />

2.   <img width="995" height="719" alt="Image" src="https://github.com/user-attachments/assets/7b963585-ade0-4da4-a9d2-1746c94c2aee" />

3.   <img width="1042" height="717" alt="Image" src="https://github.com/user-attachments/assets/76f881ab-694d-45e6-92a5-191a7dbc497d" />

