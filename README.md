# Student Performance Analysis and Prediction System

## Project Overview

This project explores how study time, absences, and earlier-period grades relate to students’ final grades. It uses a Linear Regression model to estimate a student’s final grade and flags predictions below a selected cutoff.

## Dataset

The project uses the UCI Student Performance dataset, ID 320. The dataset contains 649 records and 33 columns. The model uses `studytime`, `absences`, `G1`, and `G2` to predict `G3`.

Source: Cortez, P. (2008). [UCI Machine Learning Repository](https://doi.org/10.24432/C5TG7T).

## Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab

## How to Run

1. Open `Minor_Project_–_Student_Performance_.ipynb` in Google Colab.
2. Run the notebook cells from top to bottom.
3. The first setup cell installs `ucimlrepo`; the notebook downloads the dataset from UCI.
4. Review the charts, model predictions, and evaluation results in the notebook.

## Model and Results

The project uses Linear Regression with study time category, absences, and first- and second-period grades as inputs. On the held-out test set, MAE was 0.75, RMSE was 1.17, and R² was 0.86. The average five-fold cross-validation R² was 0.85.

## Limitations

The dataset represents students from two schools in Portugal. Study time is grouped into categories, and absences are used as a proxy for attendance. The model uses earlier grades, which are strongly related to the final grade. Predictions are estimates and should be reviewed by a person. The cutoff of 10 out of 20 is a project demonstration choice, not a school rule.

## Project Files

- `Minor_Project_–_Student_Performance_.ipynb` — code, charts, model, and findings
- `student_performance_dataset.csv` — dataset used in the project
- `Project_Report.pdf` — project report
- `README.md` — project overview and run instructions
- `screenshots/` — charts and other project evidence
