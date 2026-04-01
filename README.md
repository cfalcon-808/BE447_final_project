# BE447_final_project
Machine learning final project

Breast Cancer Survival Classification

Authors: 
Joshua Heflin(Flacon_Heflin_447_ch3_V1-2Heflin.ipynb), 
Christian Falcon(final_project1.ipynb)

This project builds a classification workflow for the breast cancer survival dataset
The goal is to predict 'patient_status' which is alive or deceased from a comabination of clinical and protein features.
There is also date data, but for now we drop those columns for prediction. The notebooks implement manual preprocessing, SVC model training, grid search and evaluation with a classification report, and confusion matrix all implemented within a python class. The DatasetClassifier class is designed to allow many different parameters like different models, na fill values, scoring, and train test splits for increased modularity and reduce the amount of code rewriting.

## Dataset
Dataset:
The primary dataset used in this project is 'breast_cancer_survival.csv'.
Target: 'Patient_Status'
Features: 'Age', 'Gender', 'Protein1', 'Protein2', 'Protein3', 'Protein4', 'Tumour_Stage', 'Histology', 'ER status', 'PR status', 'HER2 status', 'Surgery_type', 'Date_of_Surgery', 'Date_of_Last_Visit'

Date columns:'Surgery_type', 'Date_of_Surgery'

The notebook right now drops the date data, we will later figure out a way to encode the data to see if it affects the classification.

## Files:
breast_cancer_survival.csv             - primary dataset
Falcon_Heflin_447_ch3_V1-2Heflin.ipynb - Joshuas Notebook
final_project1.ipynb                   - Christians Notebook
METABRIC_RNA_Mutation.csv              - Secondary Dataset
BRCA.csv                               - Extra Dataset that I found
references:
ECE_645_Kernel_Methods_strat.ipynb     - Code reference from project from another class
A_data_preprocessing.ipynb             - Homework 2 reference

## Plan

-Improve prediction through different hyperparams and ML models.
-Compare different imputation strategies, (filling nan values with mean, median, mode, interpolation)
-add additional classifiers, and compare results
-investigate whether date features can be of use through encoding.
Unify our codes and polish them.


