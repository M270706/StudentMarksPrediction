# StudentMarksPrediction
# ML Project

# 🎓 Student Marks Prediction

## The Goal
Schools collect a lot of data on students, but usually only find out someone is struggling *after* they fail a final exam. This project uses machine learning to predict final scores early in the semester so teachers can step in and help.

## What I Did
* **Predicted Grades:** Used everyday data—like attendance and study hours—to forecast final exam scores (0–100).
* **Tested Models:** Compared five machine learning models (Linear Regression, Decision Tree, Random Forest, KNN, and Lasso) to find the most accurate one.
* **Built an App:** Created an easy-to-use web dashboard using Streamlit so teachers can easily make predictions.

## The Data
I used the `StudentPerformanceFactors.csv` dataset, which tracks various student habits. All the coding, testing, and modeling was done in Python.

## The Results: Which Model Won?
After testing the models on a hidden 20% of the data, **Linear Regression** was the clear winner! 🏆

Since the relationship between studying, showing up, and getting good grades is pretty straightforward, keeping the math simple was the smartest move.

| Model | MAE | MSE | Verdict |
| :--- | :--- | :--- | :--- |
| **Linear Regression ★** | 1.38 | 3.25 | **Best** |
| **Lasso Regression** | 1.40 | 3.31 | **Good** |
| **Random Forest** | 1.53 | 3.97 | **Moderate** |
| **KNN Regressor** | 1.54 | 3.97 | **Moderate** |
| **Decision Tree** | 1.56 | 4.27 | **Weak** |

## How to Run the Dashboard
If you want to run this project on your own computer, follow these steps:

1. Clone this repository to your machine.
2. Install the required Python libraries:
   ```bash
   pip install pandas scikit-learn streamlit plotly
3. Run the Streamlit app:
   ```bash
   streamlit run src/mini_p.py
