# AntiTbPred: Antitubercular Peptide Prediction Platform

Welcome to the official repository for AntiTbPred, a machine learning-based platform developed for predicting antitubercular peptides (AntiTbP) using sequence-derived features and ensemble classification approaches.

Web Server: http://webs.iiitd.edu.in/raghava/antitbpred/

ZENODO : https://doi.org/10.5281/zenodo.20083571

---

## Citation

Usmani, S. S., Bhalla, S., & Raghava, G. P. S. (2018).  
Prediction of Antitubercular Peptides From Sequence Information Using Ensemble Classifier and Hybrid Features.  
Frontiers in Pharmacology, 9, 954.  
https://doi.org/10.3389/fphar.2018.00954

---

## About the Platform

AntiTbPred is a computational platform developed for identifying peptides with antitubercular activity against *Mycobacterium tuberculosis*. The platform utilizes sequence-based machine learning techniques to distinguish antitubercular peptides from antibacterial and non-antibacterial peptides.

Tuberculosis remains one of the major infectious diseases worldwide, particularly due to the rise of multidrug-resistant (MDR), extensively drug-resistant (XDR), and totally drug-resistant (TDR) strains. Antitubercular peptides offer a promising alternative therapeutic strategy because of their selective affinity toward mycobacterial cell walls and reduced toxicity.

The study developed predictive models using experimentally validated antitubercular peptides and multiple sequence-derived features including amino acid composition, dipeptide composition, terminal residue composition, and binary profile patterns.

---

## Key Features

Machine Learning Models

* Support Vector Machine (SVM)
* Random Forest (RF)
* Sequential Minimal Optimization (SMO)
* Naïve Bayes
* J48 Decision Tree

Prediction Features

* Amino acid composition (AAC)
* Dipeptide composition (DPC)
* Binary profile patterns
* N-terminal and C-terminal residue composition
* Hybrid sequence features

Prediction Modules

* Antitubercular peptide prediction
* Protein sequence scanning
* Peptide analog generation
* Ensemble classification system

---

## Dataset Information

Positive Dataset

* 246 experimentally validated antitubercular peptides
* Extracted from AntiTbPdb
* Peptide lengths ranged from 5–61 amino acids

Negative Datasets

* AntiTb_MD dataset from DBAASP antibacterial peptides
* AntiTb_RD dataset from Swiss-Prot random peptides

Data Splitting

| Dataset Portion | Number of Sequences |
|---|---|
| Training Set | 199 |
| Validation Set | 47 |

---

## Important Residue Preferences

Preferred residues in antitubercular peptides:

* Lysine (K)
* Arginine (R)
* Leucine (L)
* Tryptophan (W)

Underrepresented residues:

* Aspartic acid (D)
* Glutamic acid (E)

Terminal residue analysis showed:

* R and L dominance at N-terminal positions
* L, R, and W preference at C-terminal positions

---

## Performance Summary

### Ensemble Classifier Performance

#### AntiTb_RD Dataset

| Metric | Value |
|---|---|
| Accuracy | 75.62% |
| MCC | 0.52 |
| AUROC | 0.83 |

#### AntiTb_MD Dataset

| Metric | Value |
|---|---|
| Accuracy | 73.20% |
| MCC | 0.47 |
| AUROC | 0.80 |

---

### Hybrid Model Performance

#### AntiTb_RD Dataset

| Metric | Value |
|---|---|
| Accuracy | 78.54% |
| AUROC | 0.86 |

#### AntiTb_MD Dataset

| Metric | Value |
|---|---|
| Accuracy | 75.87% |
| AUROC | 0.83 |

---

## Methodology

The prediction models were developed using:

* Five-fold cross validation
* Independent validation datasets
* Ensemble learning approaches
* Hybrid feature integration

Software & Tools Used

* SVMlight
* WEKA
* Seq2Logo

Feature Engineering

* Amino acid composition
* Dipeptide composition
* Binary encoding
* Terminal residue profiling

 
## Limitations

* Limited experimentally validated datasets
* Natural amino acids only
* Lack of experimentally verified negative peptides
* Prediction accuracy dependent on dataset diversity

---

## Contact & Authors

Prof. Gajendra P. S. Raghava  
raghava@iiitd.ac.in
IIIT DELHI

Developed at:

* Indraprastha Institute of Information Technology (IIIT Delhi), India
* CSIR-Institute of Microbial Technology, Chandigarh, India

---

## License

This work is distributed under the  
Creative Commons Attribution License (CC BY 4.0)

---

## Acknowledgements

Supported by:

* Department of Biotechnology (DBT)
* Indian Council of Medical Research (ICMR)
* J. C. Bose National Fellowship

We acknowledge all researchers contributing to antitubercular peptide research and peptide therapeutics.
