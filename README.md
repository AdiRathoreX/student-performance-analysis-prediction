
# Student Performance Analysis and Prediction System

## Project Overview

This project looks at how students spend time studying how days they skip school and what grades they had before the final exam. It then uses a math model called Linear Regression to guess the final grade. There is also a flag that highlights when the guess is below a chosen cut‑off.

## Dataset

The project uses the UCI Student Performance data set number 320. The data has 649 rows and 33 columns. The model uses the columns studytime, absences, G1 and G2 to predict the column G3.

Source: Cortez, P. (2008). UCI Machine Learning Repository. Https://doi.org/10.24432/C5TG7T

## Technologies

- Python

- Pandas and NumPy

- Matplotlib and Seaborn

- Scikit-learn

- Google Colab

## How to Run

1. Minor_project_-_student_performance.ipynb` in Google Colab.

2. Run the notebook cells from top to bottom.

3. The first setup cell installs `ucimlrepo`; the notebook downloads the dataset from UCI.

4. Review the charts, model predictions and evaluation results in the notebook.

## Model and Results

The project uses Linear Regression with study time category, absences and first- and second-period grades as inputs. On the held-out test set MAE was 0.75 RMSE was 1.17 and R² was 0.86. The average five-fold cross-validation R² was 0.85.

## Limitations

The dataset represents students from two schools in Portugal. Study time is grouped into categories and absences are used of attendance percentage. The model uses grades, which are strongly related to the final grade. Predictions are estimates. Should be reviewed by a person. The review threshold of 10, out of 20 is a project demonstration choice, not a school rule.

## Project Files

- `Minor_Project_-_Student_Performance.ipynb`. Code, charts, model and findings

- `student_performance_dataset.csv`. Dataset used in the project

- `Project_Report.pdf`. Project report

- `README.md`. Project overview and run instructions

- `screenshots/`. Evidence of charts and results
