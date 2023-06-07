# Multi-Omics Data Integration for Breast Cancer Survival Prediction

This repository contains a machine learning (ML) pipeline for the integration of large-scale omics data to predict survival outcomes in breast cancer patients. The pipeline utilizes multi-omics data, including gene expression, miRNA expression, DNA methylation, and copy number variation, from 302 female patients available in The Cancer Genome Atlas (TCGA) dataset.

## Table of Contents

- [Usage](#Usage)
- [Repository Structure](#Repository-Structure)
- [Background](#Background)
- [Objective](#Objective)
- [Model Architecture](#Model-Architecture)

## Usage
To use the ML model and run the Flask application locally, follow these steps:

1. Download the GitHub repository to your local machine.
1. Create and Activate a new python environment. 
1. Run command in terminal.
    * pip install -r requirements.txt
    * export FLASK_APP="ConnetOME.py"
    * flask run
1. Open the provided port in your preferred web browser.

## Repository Structure

This GitHub repository contains the following files and directories:

1. ConnetOME.py: The Flask application file to run the ML model.
1. models/: Directory containing the model pickle files.
1. example/: Directory containing sample example files for testing the application.


## Background
Integration of diverse omics data is crucial for extracting biologically relevant information and gaining a better understanding of the complex biological processes associated with different disease phenotypes. Machine learning approaches have shown great potential for systematic multi-omics data integration.

## Objective
The main objective of this study is to predict the survival outcomes of breast cancer patients by leveraging multi-omics data. By developing a computational ML pipeline using Support Vector Machine (SVM) and Partial Least Squares (PLS) algorithms, we aim to overcome the limitations of univariate feature selection criteria. The pipeline incorporates latent variables obtained through multivariate dimension reduction methods, allowing us to investigate background genetic networks and identify potential hub genes.

## Model Architecture
The CNN model architecture consists of several layers designed to extract features from the input images and classify them into different classes. The model architecture may vary based on the specific requirements of your project. Refer to the code documentation for details on the model architecture implemented in this project. <br>
<br>
![Alt text](image\Model_Architecture.jpg)



## Results
The analysis of the results obtained revealed that the SVM with PLS-DA method, integrated with gene expression, DNA methylation, and miRNA expression modalities, outperformed other models. It achieved an area under the curve (AUC) of 89% and an accuracy of 82% for survival prediction. Additionally, this study validated previously reported breast cancer-specific prognostic biomarkers while also predicting new biomarkers.


