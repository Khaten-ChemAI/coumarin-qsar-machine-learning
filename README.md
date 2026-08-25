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

## QSAR Analysis

The complete computational workflow is provided in the Jupyter Notebook:

**[LPS-Induced NO QSAR and Machine Learning Analysis](lps_induced_no_qsar_ml_analysis.ipynb)**

The workflow includes:

- RDKit molecular descriptor generation
- Molecular fingerprint generation
- Dataset preprocessing and pIC50 transformation
- LASSO descriptor selection
- Multicollinearity assessment
- Applicability Domain analysis
- PLS QSAR modeling
- External test-set validation
- 5-fold cross-validation
- Y-randomization validation
- VIP and descriptor coefficient analysis
- QSAR equation generation
- Residual analysis

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

## Final QSAR Model Performance

| Metric | Training Set | 5-Fold CV | External Test Set |
|---|---:|---:|---:|
| R² | 0.7820 | 0.5325 | 0.5608 |
| RMSE | 0.3119 | 0.4568 | 0.3947 |
| MAE | 0.2307 | 0.3348 | 0.3298 |
| Q² | — | 0.5325 | — |

### Model Information

- Training compounds: 27
- External test compounds: 7
- Selected descriptors: 13
- PLS components: 1
- Y-randomization permutations: 1000
- Training compounds inside AD: 25/27
- External test compounds inside AD: 6/7

### Model Validation

The final PLS QSAR model showed satisfactory agreement between observed and predicted pIC50 values, with R² = 0.7820 for the training set and R² = 0.5608 for the external test set. Five-fold cross-validation yielded Q² = 0.5325, supporting the internal predictive performance of the model. Y-randomization was performed using 1000 permutations to assess the possibility of chance correlation. The applicability domain analysis indicated that 25 of 27 training compounds and 6 of 7 external test compounds were within the defined applicability domain.

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

5. Landrum, G. **RDKit: Open-Source Cheminformatics Software.** 2016. 
   https://www.rdkit.org/

6. RDKit Documentation. **RDKit: Open-source cheminformatics toolkit.**
   https://www.rdkit.org/docs/

## Software

- **RDKit** – Molecular structure processing, molecular descriptors, fingerprints, similarity calculations, and cheminformatics workflows.  
  Landrum, G. *RDKit: Open-Source Cheminformatics Software* (2016).  
  https://www.rdkit.org/

- **scikit-learn** – Machine-learning algorithms and model validation used for QSAR modeling.  
  https://scikit-learn.org/

- **Python** – Computational programming environment used for data processing and QSAR analysis.
