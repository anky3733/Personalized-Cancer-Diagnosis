# Personalized-Cancer-Diagnosis

## 1. Description

Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/
Data: Memorial Sloan Kettering Cancer Center (MSKCC)
Download training_variants.zip and training_text.zip from Kaggle.

Context:
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/discussion/35336#198462
Problem statement : 
Classify the given genetic variations/mutations based on evidence from text-based clinical literature.

Real-world/Business objectives and constraints.
No low-latency requirement.
Interpretability is important.
Errors can be very costly.
Probability of a data-point belonging to each class is needed.

## 2. Data

 ### 2.1 Data Overview
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment/data
We have two data files: one contains the information about the genetic mutations and the other contains the clinical evidence (text) that human experts/pathologists use to classify the genetic mutations.
Both these data files are have a common column called ID
Data file's information:
training_variants (ID , Gene, Variations, Class)
training_text (ID, Text)

### 2.2. Mapping the real-world problem to an ML problem

#### 2.2.1. Type of Machine Learning Problem
There are nine different classes a genetic mutation can be classified into => Multi class classification problem

#### 2.2.2. Performance Metric
Source: https://www.kaggle.com/c/msk-redefining-cancer-treatment#evaluation
Metric(s):
Multi class log-loss
Confusion matrix

