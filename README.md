# Student Performance Analysis and Score Prediction

This project explores student performance data and uses a simple linear regression model to estimate a student's final score from their weekly study hours. The analysis is in a Jupyter notebook and uses the included CSV dataset.

## Project files

- `project.ipynb` — data exploration, score visualization, linear regression, evaluation metrics, and an example prediction.
- `student_performance_updated_5000.csv` — student performance dataset.

## Requirements

- Python 3
- Jupyter Notebook
- pandas
- scikit-learn
- matplotlib
- NumPy

Install the Python packages with:

```bash
pip install jupyter pandas scikit-learn matplotlib numpy
```

## Run the notebook

1. Clone or download this repository.
2. Open a terminal in the project directory.
3. Start Jupyter:

   ```bash
   jupyter notebook
   ```

4. Open `project.ipynb` and run its cells. Keep the CSV in the same directory as the notebook so it can be loaded by the notebook.

## What the notebook does

1. Loads the CSV data with pandas.
2. Uses `study_hours_per_week` as the input feature and `final_score` as the target.
3. Fits a scikit-learn `LinearRegression` model.
4. Plots the distribution of final scores and the regression predictions against the observed scores.
5. Reports mean absolute error (MAE), mean squared error (MSE), root mean squared error (RMSE), and R².
6. Demonstrates a score prediction for 9 study hours per week.

## Notes

The notebook currently fits and evaluates the model on the same data, without a separate test set. Its reported metrics therefore measure fit on the training data and do not show how well the model generalizes to unseen students. The prediction is a simple demonstration based on study hours alone; it should not be treated as a guaranteed result.

## Dataset columns

The CSV includes student identifiers and demographic, academic, and performance fields, including study hours, attendance, midterm scores, final scores, assignment and quiz scores, participation, project scores, total score, and grade.
