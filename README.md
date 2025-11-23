📘 IBM SPSS Modeler Project – Diabetes Analysis & Customer Segmentation

A complete GitHub‑style README for the SPSS Modeler workflow you created.


---

📌 Project Overview

This project uses IBM SPSS Modeler to perform:

Diabetes Prediction (Classification)

Customer Segmentation (optional extension)


The workflow includes data import, field type assignment, filtering, partitioning, modeling, and evaluation.


---

📂 Repository Structure

📁 project-folder
│── 📄 README.md       → Project documentation
│── 📁 data/           → Dataset files (CSV/Excel)
│── 📁 screenshots/    → SPSS Modeler workflow images
│── 📁 exports/        → Model outputs (tables, graphs)


---

🧩 SPSS Modeler Workflow Summary

The workflow includes the following nodes:

      1. Data Source Node (Var. File / Excel / CSV)

Imports dataset with all fields.

      2. Type Node

Assigns correct data types and roles:

     Input Fields

     Target Field (Outcome)

     Continuous / Nominal Levels


     3. Select Node

Filters unnecessary or missing records. Example filter:

   @NOT(@NULL(Glucose)) AND @NOT(@NULL(BMI))

    4. Partition Node

Splits dataset:

                  70% Training

                   30% Testing
                Used for model evaluation.

5. Modeling Nodes

Multiple algorithms are applied:

C5.0 Decision Tree

Logistic Regression

SVM (Support Vector Machine)


Each model predicts the Outcome variable.

6. Analysis Nodes

Evaluates and compares model performance using:

ROC Curve

Confusion Matrix

Accuracy Score

Model Summary Reports



---

🧪 Model Evaluation Example

Model: C5.0 Decision Tree
Accuracy: 78.4%
AUC: 0.82
Confusion Matrix:
TP: 120 | FP: 30
FN: 25  | TN: 89

(Your results may differ depending on dataset)


---

🔧 Dataset Fields

Example fields used:

Pregnancies
Glucose\ nBloodPressure
SkinThickness
Insulin
BMI
DiabetesPedigreeFunction
Age
Outcome (Target)


---

🛠 Setup Instructions

Requirements

IBM SPSS Modeler (any recent version)

Dataset (CSV/Excel)


Steps

1. Open SPSS Modeler


2. Drag a Var. File node and import dataset


3. Apply Type Node to correct field types


4. Use Select Node to clean/prepare data


5. Apply Partition Node


6. Add modeling nodes (C5.0 / Logistic / SVM)


7. Add Analysis Node to compare models




---

📊 Result Interpretation

Higher accuracy or AUC means better model.
Choose the model with:

Highest ROC AUC

Best Confusion Matrix

Lowest Misclassification Rate



---

📝 Sample README Code Block

# Diabetes Prediction using IBM SPSS Modeler
This project builds classification models using the PIMA Diabetes dataset.

## Features
- Data Import
- Partitioning
- C5.0 Model
- Logistic Regression
- SVM
- Model Evaluation (Accuracy, ROC, Confusion Matrix)


---

🤝 Contributions

Feel free to fork and modify the README or stream.


---

📬 Author

Suraj Kumar
B.Tech CSE (AI & DS) – 5th Semester
Arka Jain University


