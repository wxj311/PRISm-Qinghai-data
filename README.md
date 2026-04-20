PRISm-Qinghai-data

De-identified dataset, data dictionary, and supporting documentation for the study:

Construction and Validation of a Risk Prediction Model for Preserved Ratio Impaired Spirometry (PRISm) in the Western Qinghai Plateau Region

Repository link: https://github.com/wxj311/PRISm-Qinghai-data



 Overview

This repository provides the de-identified analysis dataset and supporting files for a study on risk prediction of preserved ratio impaired spirometry (PRISm) in adults living in the western Qinghai plateau region, China.

The repository includes:

 a standardized numeric dataset for statistical analysis,
 a labeled dataset for human-readable review,
 a data dictionary describing variables and coding,
 a quality-control review file for records requiring manual verification,
 and an Excel summary package for convenient inspection.

These files are shared to support transparency, reproducibility, and secondary academic use.



 Repository structure

text
PRISm-Qinghai-data/
├─ data/
│  ├─ prism64_standardized_numeric.csv
│  ├─ prism64_standardized_labeled.csv
│  ├─ data_dictionary.csv
│  └─ qc_review_flags.csv
├─ docx/
│  └─ PRISM64_standardized_package.xlsx
└─ README.md
Files
data/prism64_standardized_numeric.csv

The main de-identified analysis dataset.
Variable names are standardized in lowercase snake_case format and are suitable for use in R, Python, SPSS, or other statistical software.

data/prism64_standardized_labeled.csv

A human-readable version of the dataset.
Categorical values are presented using descriptive labels to facilitate manual review.

data/data_dictionary.csv

The variable dictionary for the dataset.
This file includes variable names, labels, coding rules, and brief descriptions.

data/qc_review_flags.csv

A quality-control review file listing records that should be manually checked before formal downstream analysis or external reuse.

docs/PRISM64_standardized_package.xlsx

An Excel package containing the standardized dataset and related supporting tables for quick inspection.

Study summary

This dataset was derived from a high-altitude screening study conducted in the western Qinghai plateau region. The study focused on identifying and evaluating risk factors associated with PRISm.

PRISm was defined as:

FEV1/FVC ≥ 0.70, and
FEV1 % predicted < 80% and/or FVC % predicted < 80%

The shared dataset is de-identified and intended for research transparency and reproducibility.

Data processing and standardization

The dataset was processed before release using the following principles:

De-identification
Direct personal identifiers were removed. A study-specific anonymous ID was added for each record.
Standardized variable names
Column names were converted to lowercase snake_case format.
Consistent coding
Binary and categorical variables were standardized to improve interoperability across software platforms.
Unit normalization
Variables with unit inconsistencies were harmonized where appropriate.
Quality-control flags
Potentially inconsistent or unusual values were listed separately in qc_review_flags.csv for manual review.
Important note for users

Please review qc_review_flags.csv before conducting formal secondary analyses.
Although the dataset has been standardized, some records were intentionally retained with QC flags rather than being automatically altered.

Users should also consult data_dictionary.csv before analysis to ensure correct interpretation of variable coding and units.

Suggested use

This repository may be used for:

replication of the published analyses,
sensitivity analyses,
educational purposes,
and methodological research on PRISm-related prediction modeling.
Data availability statement

The de-identified dataset, data dictionary, and QC notes supporting the findings of this study are publicly available in the GitHub repository “PRISm-Qinghai-data” at:

https://github.com/wxj311/PRISm-Qinghai-data

Citation

If you use this dataset, please cite the associated article and acknowledge this GitHub repository.

Suggested citation format:

De-identified dataset for the PRISm study in the western Qinghai plateau region. GitHub repository: https://github.com/wxj311/PRISm-Qinghai-data

Contact

For questions regarding the dataset or requests for clarification, please contact the corresponding author(s) listed in the manuscript.

Disclaimer

This repository contains a de-identified research dataset intended for academic and scientific use only.
Users are responsible for ensuring appropriate interpretation, analysis, and citation of the data.
