# student-risk-classification
A machine learning classification project to identify students who may be academically at risk using structured classroom data. Built with a custom dataset, basic EDA, and simple models, with focus on recall to avoid missing students who need early support.
# Student Risk Prediction using Machine Learning

## Overview
This project focuses on identifying students who are academically at risk using
structured academic and behavioral data.  
The goal is early identification so that timely intervention can be planned.

This project was built as part of my learning journey while transitioning from
a Physics educator role into the AI/ML domain, with emphasis on fundamentals
and decision-oriented machine learning.

---

## Problem Statement
The task is framed as abinary classification problem:

> Predict whether a student is **at academic risk** or **not at risk**

 `1` → At Risk (needs intervention)  
 `0` → Not At Risk  

The focus is not only on prediction, but on understanding how different academic
factors contribute to risk.



# Dataset
A custom synthetic dataset was created to simulate realistic classroom scenarios.
The dataset represents a snapshot of student performance and behavior.

# Features
- **Attendance (%)** – class participation indicator  
- **Study hours (per week)** – effort and consistency  
- **Assignment submission rate (%)** – engagement with coursework  
- **Average test score** – academic performance indicator  
- **Engagement level** – low / medium / high (encoded numerically)

# Target
 at_risk  
  - `1` → student needs academic intervention  
  - `0` → student is performing satisfactorily  

The dataset is intentionally **imbalanced** to reflect real-world conditions
where fewer students are at high risk.

---

## Exploratory Data Analysis (EDA)
The following analyses were performed:
- Distribution of at-risk vs not-at-risk students
- Correlation analysis between academic features
- Visualization of feature relationships using heatmaps and count plots

EDA helped confirm which factors are most strongly associated with academic risk.

---

## Models Used
The following machine learning models were implemented and compared:
- Logistic Regression (baseline model)
- Decision Tree Classifier
- Random Forest Classifier

Models were chosen for simplicity, interpretability, and suitability for a beginner-level project.

---

## Evaluation Metrics
Model performance was evaluated using:
- Accuracy
- Confusion Matrix
- Precision, Recall, and F1-score

Special emphasis was placed on **recall for the at-risk class**, as failing to identify
a student who needs help is more costly than a false alarm.



# Key Learnings
- Framing real-world problems as classification tasks
- Designing a dataset using domain knowledge
- Handling class imbalance using class weighting
- Understanding why accuracy alone is not sufficient
- End-to-end ML workflow from data creation to evaluation


# Limitations
- The dataset is synthetic and created for learning purposes
- No temporal or longitudinal data is included
- Results may not generalize directly to real institutions without validation

---

# Future Improvements
- Use a real-world dataset for validation
- Add feature importance analysis
- Experiment with threshold tuning
- Deploy a simple interface for predictions

# Author
Ishan  

