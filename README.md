# QSAR and Machine Learning Analysis of Coumarin-Based Compounds Against LPS-Induced NO Production

## Overview

This repository contains an exploratory Quantitative Structure–Activity Relationship (QSAR) and machine learning analysis of coumarin-based compounds evaluated for biological activity against LPS-induced nitric oxide (NO) production.

The study explores the application of cheminformatics and machine learning approaches to investigate relationships between molecular structure and biological activity.

## Objectives

* Prepare and explore a biological activity dataset.
* Generate molecular representations using RDKit.
* Calculate molecular fingerprints and molecular descriptors.
* Investigate molecular similarity and chemical space.
* Develop and compare machine learning models for QSAR analysis.
* Evaluate model performance using appropriate statistical metrics.

## Computational Workflow

1. **Dataset Preparation**
2. **Data Preprocessing**
3. **Molecular Fingerprint Generation**
4. **Molecular Descriptor Calculation**
5. **Chemical Space and Similarity Analysis**
6. **Machine Learning Model Development**
7. **Model Evaluation**

## Tools and Technologies

* Python
* RDKit
* Pandas
* NumPy
* Scikit-learn
* Matplotlib

## Current Analysis

The current notebook contains the initial QSAR and machine learning workflow, including molecular representation, data analysis, model development, and evaluation of predictive performance.

This repository represents an ongoing computational study, and the analysis may be updated as the dataset, molecular descriptors, feature selection, and machine learning approaches are further optimized.

## Repository Contents

* `lps_induced_no_qsar_ml_analysis.ipynb` — Jupyter Notebook containing the QSAR and machine learning analysis.

## Future Work

Future improvements may include:

* Dataset expansion and curation
* Descriptor selection and feature engineering
* Hyperparameter optimization
* Cross-validation and external validation
* Comparison of additional machine learning algorithms
* Improved model interpretability

## Note

This is an exploratory research project developed for investigating QSAR and machine learning approaches to coumarin-based compounds. The reported models should be interpreted in the context of the available dataset and validation strategy.

## Dataset

The dataset comprises 34 coumarin-based compounds with experimentally reported
pIC50 values for inhibition of LPS-induced nitric oxide (NO) production.

The activity data were compiled from previously published literature. Each
compound and its corresponding biological activity were curated from the
reported experimental data and transformed to pIC50 values for QSAR analysis.

### Data Sources

Literature sources used in the dataset are:

1. Liu, Y.-P.; Yan, G.; Xie, Y.-T.; Lin, T.-C.; Zhang, W.; Li, J.; Wu, Y.-J.; Zhou, J.-Y.; Fu, Y.-H. Bioactive prenylated coumarins as potential anti-inflammatory and anti-HIV agents from *Clausena lenis*.*Bioorganic Chemistry* **2020**, 97, 103699.

DOI: https://doi.org/10.1016/j.bioorg.2020.103699

2. Fattah, T. A.; Saeed, A.; Al-Hiari, Y. M.; Kasabri, V.; Almasri, I. M.; AlAlawi, S.; Larik, F. A.; Channar, P. A. Functionalized Furo[3,2-c]coumarins as Anti-Proliferative, Anti-Lipolytic, and Anti-Inflammatory Compounds: Synthesis and Molecular Docking Studies. *J. Mol. Struct.* **2019**, *1179*, 390–400. 

DOI: https://doi.org/10.1016/j.molstruc.2018.11.014

3. Wei, W.; Wu, X.-W.; Deng, G.-G.; Yang, X.-W. Anti-inflammatory Coumarins with Short- and Long-Chain Hydrophobic Groups from Roots of *Angelica dahurica* cv. Hangbaizhi. *Phytochemistry* **2016**, *123*, 58–68.

DOI: https://doi.org/10.1016/j.phytochem.2016.01.006.

4. Liang, H.; Shi, Y.; Zeng, K.; Zhao, M.; Tu, P.; Jiang, Y. Coumarin derivatives from the leaves and twigs of *Murraya exotica* L. and their anti-inflammatory activities. *Phytochemistry* **2020**, *177*, 112416.

DOI: https://doi.org/10.1016/j.phytochem.2020.112416.
