# Coursework Project: Data Preparation and Model Performance Analysis
## Overview
This repository contains the coursework project focusing on implementing various data preparation techniques and their impact on model performance. The project involved taking a dataset, applying 25 different data preparation techniques, training a model with the updated dataset, and evaluating the model's performance.

# Project Structure
archive/: Contains the original dataset and its modified versions of the dataset. This dataset was taken from Kaggle

data_preperation_project.ipynb: Source code for data preparation, model training, and performance evaluation. This has all the project code.

project definition (Graduate).pdf: Jupyter notebooks demonstrating the step-by-step process of the project.

## Summary

Using data preparation, we improved the model from 57.23 to 85.54

There is a **28.31 points increase from baseline to best model**

|Experiment                                    |Description                      |Score |Improvement|Comment   |
|:--------------------------------------------:|:-------------------------------:|:----:|:---------:|:--------:|
|                   **Baseline**                   |            Baseline             |**57.23** |     -     |Baseline 1|
|             **Duplicate Instances**              |                                 |      |           |          |
|                    Exp 1                     |  Handling Duplicate Instances   |67.09 |   +9.86    |Baseline 2|
|           **Missingness in features**            |                                 |      |           |          |
|                    Exp 2                     |        Mean substitution        |66.98 |   -0.11   |          |
|                    Exp 3                     |       Median substitution       |66.98 |   -0.11   |          |
|                    Exp 4                     |     Frequency Substitution      |66.98 |   -0.11   |          |
|                    Exp 5                     |       Multiple Imputation       |67.46 |   +0.37    |          |
|                    Exp 6                     |           kNN imputer           |69.42 |   +2.33    |Baseline 3|
|              **Compound Variables**              |                                 |      |           |          |
|                    Exp 7                     |   Handling Compound Variables   |77.12 |    +7.7    |Baseline 4|
|              **Outlier Detection**               |                                 |      |           |          |
|                    Exp 8                     |      kNN outlier detection      |73.42 |   -3.7    |          |
|                    Exp 9                     |        Isolation Forest         |77.97 |   +0.85    |Baseline 5|
|   **Feature Transformation - Discretization**    |                                 |      |           |          |
|                    Exp 10                    |     Interval Based Binning      |78.29 |   +0.32    |Baseline 6|
|                    Exp 11                    |     Frequency Based Binning     |77.57 |   -0.4    |          |
|                    Exp 12                    |     Threshold Based Binning     |76.33 |   -1.64   |          |
|          **1:1 Feature Transformation**          |                                 |      |           |          |
|                    Exp 13                    |            Centering            |78.27 |   -0.02   |          |
|                    Exp 14                    |             Scaling             |78.25 |   -0.04   |          |
|                    Exp 15                    |        Standard Scaling         |78.28 |   -0.01   |          |
|        **1:many Feature Transformation**         |                                 |      |           |          |
|                    Exp 16                    |         Basis Expansion         |78.27 |   -0.02   |          |
|                    Exp 17                    |        One Hot Encoding         |78.16 |   -0.13   |          |
|                    Exp 18                    |             Hashing             |78.16 |   -0.13   |          |
|                    Exp 19                    |Encoding Interval/Ratio Variables|78.16 |   -0.13   |          |
| **Many:Many Transformation - Feature Expansion** |                                 |      |           |          |
|                    Exp 20                    |Kernel-Induced Feature Expansion |46.14 |  -32.15   |          |
|**Many:Many Transformation - Feature Contraction**|                                 |      |           |          |
|                    Exp 21                    |               PCA               |49.52 |  -28.77   |          |
|                    Exp 22                    |              t-SNE              |49.79 |   -28.5   |          |
|                    Exp 23                    |        Isometric Mapping        |59.22 |  -19.07   |          |
|              **Feature Selection**               |                                 |      |           |          |
|                    Exp 24                    |  Sequential Forward Generation  |84.81 |   +6.52    |          |
|                    Exp 25                    | Sequential Backward Generation  |**85.54** |   +7.25    |**BEST MODEL**|
