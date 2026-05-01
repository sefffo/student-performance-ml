# Student Performance ML

Machine Learning project for predicting student final grade (G3) using the Student Performance Dataset.

## Contents
- `student_performance_model.ipynb` — full Jupyter notebook
- Multiple model comparison
- Best model selection
- Overfitting detection using train/test gap and learning curves
- Unit test cases for model validation

## Dataset
Source: [Kaggle Student Performance Dataset](https://www.kaggle.com/datasets/devansodariya/student-performance-data)

This project uses the math student dataset (`student-mat.csv`) and predicts the final grade `G3`.

## Models Compared
- Linear Regression
- Ridge
- Lasso
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- KNN Regressor
- SVR

## What the notebook does
1. Loads and explores the dataset
2. Encodes categorical features
3. Splits train/test data
4. Compares several algorithms
5. Selects Random Forest as the best model
6. Checks for overfitting
7. Draws learning curves
8. Creates feature importance charts
9. Runs 10 test cases with `unittest`

## How to run
1. Download the dataset from Kaggle
2. Place `student-mat.csv` next to the notebook
3. Run the notebook cells in order

## Kaggle download
```bash
kaggle datasets download -d devansodariya/student-performance-data --unzip
```

## Notes
- The exact best algorithm can vary slightly depending on train/test split.
- In many student performance datasets, tree-based ensembles like Random Forest often perform very well.
