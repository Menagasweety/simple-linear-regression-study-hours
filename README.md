# Simple Linear Regression: Study Hours vs Exam Scores

## Project Overview

This beginner-friendly Machine Learning project uses Simple Linear Regression to explore the relationship between students' study hours and exam scores.

The model learns a linear relationship from training data and predicts exam scores based on study hours.

## Objectives

- Understand the Simple Linear Regression workflow.
- Explore and prepare a real dataset.
- Train and test a regression model.
- Compare the model against a baseline.
- Evaluate predictions using MAE, RMSE, and R².
- Visualize the regression line and analyze residuals.
- Generate predictions for new inputs.

## Dataset

The dataset contains 200 observations and 6 columns. This project uses two columns:

- `hours_studied`: Input feature (independent variable).
- `exam_score`: Target variable (dependent variable).

The dataset was checked for missing values and duplicate records before modeling. No missing values or duplicate records were found in the dataset.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Methodology

1. Loaded and inspected the dataset.
2. Selected study hours as the input feature and exam score as the target.
3. Split the data into training and testing sets using an 80:20 ratio.
4. Created a mean-based baseline model.
5. Trained a Simple Linear Regression model.
6. Generated predictions for the test set.
7. Evaluated both models using MAE, RMSE, and R².
8. Visualized the regression line.
9. Analyzed residuals.
10. Generated predictions for new study-hour inputs.

## Regression Equation

**Predicted Exam Score = 23.78 + (1.61 × Study Hours)**

The intercept is approximately 23.78, and the slope is approximately 1.61. Within the fitted linear model, each additional study hour corresponds to an estimated increase of about 1.61 score points.

## Model Evaluation

| Metric | Baseline Model | Simple Linear Regression |
|---|---:|---:|
| MAE | 6.120 | 3.827 |
| RMSE | 7.303 | 4.378 |
| R² Score | -0.005 | 0.639 |

### Results

- The Linear Regression model achieved a lower MAE and RMSE than the baseline model.
- The test-set R² score was 0.639, indicating that the model explained approximately 63.9% of the variation in exam scores on this test split.
- The results suggest that study hours provide useful predictive information for this dataset.

## Limitations

- Only one input feature was used.
- Other factors influencing exam performance were not included.
- The relationship does not prove that additional study hours cause a specific score increase.
- Results may vary with different data samples.
- Predictions outside the observed range of study hours may be unreliable.

## How to Run the Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Ensure the CSV file is placed in the expected `data/` directory.
5. Run the notebook cells in order.

## Future Improvements

- Add more relevant student-performance features.
- Compare Simple Linear Regression with other regression models.
- Validate the model with additional data or cross-validation.
- Investigate residual patterns and regression assumptions.

## Learning Outcome

This project demonstrates the end-to-end workflow of a basic regression problem, including data preparation, model training, evaluation, visualization, and prediction.

**Note:** This is an educational project and is not intended to make high-stakes decisions about students.
