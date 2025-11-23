IBM SPSS Modeler Project – README

📌 Project Title

Diabetes Analysis and Customer Segmentation Using IBM SPSS Modeler


---

📖 Overview

This README explains the SPSS Modeler stream shown in the workflow. It describes each node, its function, and how the overall process works.


---


🧩 SPSS Modeler Workflow Explanation

Below is the detailed explanation of every node used in your SPSS Modeler workflow:

1. Data Source Node (Var. File / Excel / CSV)

This node imports the dataset (Diabetes Dataset or Happiness Dataset). It reads all records and fields.

2. Type Node

The Type node is used to assign the correct measurement level to each variable, such as:

Numeric

Categorical

Flag

Continuous / Nominal


It also allows you to set the role for each field like Input, Target, Both, None.

3. Select Node

This node filters the data. You can use conditions like:

Outcome = 0 or Outcome = 1

Or remove missing values.

4. Partition Node

This node splits the dataset into:

Training Data (typically 70%)

Testing Data (typically 30%)


This helps in model building and evaluating performance.

5. Modeling Nodes

In the picture, multiple modeling techniques are used:

a. C5.0 Decision Tree

Generates a classification tree model based on input predictors.

b. Logistic Regression

Statistical model used to predict binary outcomes like 0/1.

c. SVM (Support Vector Machine)

A powerful classification method that identifies best separating boundaries.

Each model predicts Outcome.

6. Analysis Nodes

These nodes evaluate the prediction performance using:

Accuracy

ROC Curve

Confusion Matrix

Model Comparison



---

📄 Sample README Code (Markdown Format)

# SPSS Modeler Workflow – Diabetes Prediction

## Steps Used
1. Load Dataset
2. Define Field Types
3. Filter Data with Select Node
4. Partition into Train/Test
5. Build Models (C5.0, Logistic Regression, SVM)
6. Compare Accuracy
7. Generate Analysis Outputs

## Field Roles
- Input: Pregnancies, Glucose,
