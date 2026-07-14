# HL_DHL — Analysis code

Analysis code for:

Maurud S, Lunde L, Moen A, Opheim R. Mapping conditional health literacy and
digital health literacy in patients with inflammatory bowel disease to optimise
availability of digital health information: a cross-sectional study.
Scandinavian Journal of Gastroenterology. 2025;60(6):536–47.
https://doi.org/10.1080/00365521.2025.2497952

## Contents

- `HL_DHL_analyses.Rmd` — full analysis workflow (data preparation, descriptive
  statistics, canonical correlation analysis, cluster analyses)
- `HL_DHL_analyses.pdf` — rendered version of the above
- `List of packages used in R.pdf` — R packages and versions

## Data availability

The underlying patient data are not publicly available due to privacy
regulations and the terms of the ethics approval. The code is shared to
document the analytical workflow. Data access requests are described in the
published article.

## Software and packages

Analyses were conducted in R (version 4.4.1). Full package references
are provided in `Packages used in R.pdf`.

| Package | Purpose |
|---|---|
| dplyr | Data transformation |
| impute | Imputing missing values (k-nearest neighbour averaging) |
| candisc | Canonical correlation analysis |
| car | Variance inflation factors |
| caret | k-fold cross-validation; training and evaluating the logistic model |
| foreach, doParallel | Parallel execution of jackknife iterations |
| reshape2 | Reshaping data frames for plotting |
| cluster | Agglomerative coefficients across linkage/distance combinations |
| NbClust | Determining the optimal number of clusters |
| fpc | Cluster stability assessment |
| MASS | Multivariate normal simulation for significance testing of cluster assignments |
| MKinfer | Permuted t-tests |
| pROC | ROC-AUC for the logistic model |
| coin | Permutation test of the logistic model |
| ggplot2, ggdendro, extrafont | Visualisation |
