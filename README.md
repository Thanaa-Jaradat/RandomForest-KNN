🩺 Diabetes Prediction Using KNN & Random Forest
This project uses a dataset of medical records to predict whether someone has diabetes. It walks through cleaning the data, choosing the most important features, and testing how well the K-Nearest Neighbors (KNN) model works with different settings.

📊 What’s in the Data?
The dataset (pima-indians-diabetes.csv) includes health info like:

Number of pregnancies

Blood pressure

Blood sugar levels

Skin thickness

Insulin levels

BMI (body mass index)

Age

Whether the person has diabetes (class column)

🧹 What the Code Does
Cleans the Data

Some values were incorrectly marked as 0 (like blood pressure or insulin). These were replaced with the average value instead.

Outliers (unusual values) were removed to make the data more reliable.

Splits the Data

The data is split into training, validation, and testing sets to check how well the model performs.

Finds Important Features

A Random Forest model helped to figure out which columns were most useful. The top 3 were:

Plasma glucose

BMI

Age

Tests KNN with Different Settings

Tried different values of k (1 to 3) to see which gives the best results.

For each value, it was checked how well the model did on training, validation, and testing sets.

Shows the Results

It prints out confusion matrices (which show correct vs. incorrect predictions) and classification reports (with accuracy, precision, recall).

It also creates a nice plot to visualize how KNN makes decisions based on the data.

📌 How to Run It
Make sure the file 'pima-indians-diabetes.csv' is in the same folder.

Install the required Python libraries:
pip install pandas numpy matplotlib seaborn scikit-learn scipy

Run the Python script:
python your_script_name.py

📷 Output
You’ll see:

A table showing how many invalid zero values were fixed.

Plots for:

Outliers

Feature importance

KNN decision boundary

Accuracy scores and confusion matrices for different settings.

🧠 Why This Matters
By the end of the script, we get a good idea of which medical factors are most helpful in predicting diabetes and how KNN performs with them. It’s a great intro to working with real-world data and testing machine learning models.