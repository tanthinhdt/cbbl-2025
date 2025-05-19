# Cytotoxicity of Nanoparticles

## Introduction

This report investigates the prediction of nanoparticle cytotoxicity using the TabPFN-v2 model, a state-of-the-art architecture for tabular data. I explore the optimization of the data pipeline and TabPFN-v2 model to achieve optimal predictive performance on a nanoparticle cytotoxicity dataset.

## File Structure

```text
.
└── cbbl-2025/
    │
    ├── classification/                     <-- Experiments for classification task
    │   ├── c_decision-tree.ipynb           <-- Experiment for decision tree
    │   ├── c_gradient-boosting.ipynb       <-- Experiment for gradient boosting
    │   ├── c_logistic-regression.ipynb     <-- Experiment for logistic regression
    │   ├── c_random-forests.ipynb          <-- Experiment for random forests
    │   ├── c_tabpfn-v2-90.ipynb            <-- Experiment for TabPFN-v2 with 90% data
    │   ├── c_tabpfn-v2-optimized.ipynb     <-- Experiment for optimized TabPFN-v2
    │   ├── c_tabpfn-v2.ipynb               <-- Experiment for TabPFN-v2
    │   ├── c_tabpfn-v2_exp.ipynb           <-- Experiments for data pipeline
    │   ├── test.csv                        <-- Test set for classification task
    │   └── train.csv                       <-- Train set for classification task
    │
    ├── images/                         <-- visualizations for the report and slide
    │   ├── feature_importance.png      <-- visualizations for featrue importance
    │   ├── tabpfn-v2_classifier.png    <-- visualizations for TabPFN-v2 classifier 
    │   ├── tabpfn-v2_regressor.png     <-- visualizations for TabPFN-v2 regressor 
    │   ├── target_visualization.png    <-- visualizations for regression Target variable
    │   └── target_visualization_after_handling_outliers.png    <-- visualizations for regression Target variable after handling outliers
    │
    ├── regression/                         <-- Experiments for regression task
    │   ├── r_bio-gpt.ipynb                 <-- Experiment for BioGPT
    │   ├── r_decision-tree.ipynb           <-- Experiment for decision tree
    │   ├── r_gpt2.ipynb                    <-- Experiment for GPT2
    │   ├── r_gradient-boosting.ipynb       <-- Experiment for gradient boosting
    │   ├── r_linear-regression.ipynb       <-- Experiment for linear regression
    │   ├── r_llama3.ipynb                  <-- Experiment for Llama 3.1 8B
    │   ├── r_random-forests.ipynb          <-- Experiment for random forests
    │   ├── r_tabpfn-v2-90.ipynb            <-- Experiment for TabPFN-v2 with 90% data
    │   ├── r_tabpfn-v2-optimized.ipynb     <-- Experiment for optimized TabPFN-v2
    │   ├── r_tabpfn-v2.ipynb               <-- Experiment for TabPFN-v2
    │   ├── r_tabpfn-v2_exp.ipynb           <-- Experiments for data pipeline
    │   ├── test.csv                        <-- Test set for regression task
    │   └── train.csv                       <-- Train set for regression task
    │
    ├── results/                        <-- Experiment results
    │   ├── dimensionality_reduction    <-- Experiment results on dimensionality reduction
    │   ├── feature_encoding            <-- Experiment results on feature encoding
    │   ├── feature_scaling             <-- Experiment results on feature scaling
    │   ├── main                        <-- Main experiment results
    │   ├── missing_values              <-- Experiment results on missing values handling
    │   └── outliers                    <-- Experiment results on outliers handling
    │
    ├── .gitignore          <-- Files or patterns to ignore
    ├── README.md           <-- Introduction of this project. YOU ARE HERE!
    └── requirements.txt    <-- Dependencies for this project
```
