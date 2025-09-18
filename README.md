Overview

This project explores a dataset (CSV format, e.g., from Kaggle or UCI Machine Learning Repository) using Python, Pandas, Matplotlib, and Seaborn.
It performs:

Data loading and inspection

Handling missing values

Basic statistics and grouping analysis

Data visualization (line, bar, histogram, scatter)

Optional saving of results and plots

If no dataset is provided, the script falls back to the Iris dataset from scikit-learn.

📂 Files

main.py → Main Python script (your code).

cleaned_dataset.csv → Output file with missing values handled.

dataset_describe.csv → Summary statistics of the dataset.

(Optional) /plots/ → Folder where generated plots can be saved if enabled.

⚙️ Requirements

Install dependencies before running:

pip install pandas numpy matplotlib seaborn scikit-learn

▶️ How to Run
1. Use a Local CSV Dataset (e.g., Kaggle download)

Update the csv_path in main.py:

csv_path = r"C:\Users\Admin\Downloads\your_dataset.csv"


Run the script:

python main.py

2. Use the Default Iris Dataset

If you don’t set a csv_path, the script will automatically load the Iris dataset:

csv_path = None

📊 Features
🔹 Data Exploration

Displays the first rows of the dataset

Shows data types, missing values, and summary statistics

🔹 Data Cleaning

Handles missing values using strategies:

median (default)

mean

mode

constant

drop (removes rows with missing values)

🔹 Basic Analysis

Descriptive statistics (.describe())

Grouping by categorical variables and computing averages

🔹 Visualization (Matplotlib & Seaborn)

Generates:

Line chart – Trends over time (or pseudo-time if no datetime column)

Bar chart – Average values across categories

Histogram – Distribution of a numeric column

Scatter plot – Relationship between two numeric columns

(Optional) Seaborn Pairplot for quick numeric overview

All plots include titles, labels, and legends.

📤 Outputs

After running:

✅ cleaned_dataset.csv → Cleaned dataset

✅ dataset_describe.csv → Summary statistics

✅ Visualizations → Shown on screen (and saved to /plots/ if save_plots=True)

🚀 Next Steps

Replace with any Kaggle dataset you download.

Adjust the cleaning strategy depending on your dataset.

Extend the code with additional visualizations (heatmaps, boxplots, etc.).
