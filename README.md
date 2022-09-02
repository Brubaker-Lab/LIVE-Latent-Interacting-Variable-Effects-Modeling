# LIVE-Latent-Interacting-Variable-Effects-Modeling

## Abstract
Latent Interacting Variable Effects (LIVE) modeling framework integrates different types of microbiome multi-omics data by combining discriminative latent variables from single-omic sPLS-DA models into a structured meta model to determine the most discriminative interacting multi-omics features drive disease status. LIVE modeling was implemented in publicly available metagenomic and metabolomics data set from Crohn’s Disease and Ulcerative Colitis status patients in the PRISM and LLDeep cohorts. Here, LIVE modeling framework reduced the number of feature correlations from the original data set for CD and UC (>1.62 x 109 microbe-metabolites-microbial enzymes pairs) to tractable numbers (CD=7,562 and UC=2,271, VIP>1, q < 0.01), and facilitated prioritization of biological associations between microbes, metabolites, enzymes and IBD status through the application of stringent thresholds using generated inferential statistics. We determined LIVE modeling predicted features previously reported, and uncovers more feature interactions that increase the likelihood to establish testable hypothesis and studying biological mechanisms in IBD. LIVE modeling makes a distinct and complementary contribution to the current methods to integrate microbiome data to predict IBD status because of its flexibility to adapt to different types of microbiome multi-omics data, scalability for large and small cohort studies via reliance on latent variables and dimensionality reduction, and the intuitive interpretability of the linear meta-model integrating -omic data types. The results of LIVE modeling and the biological relationships can be represented in networks that connect local correlation structure of single omic data types with global community and omic structure in the latent variable VIP scores. This model arises as novel tool that allows researchers to be more selective about omic feature interaction without disrupting the structural correlation framework provided by sPLS-DA interaction effects modeling. It will lead to form testable hypothesis by identifying potential and unique interactions between metabolome and microbiome that must be considered for future studies. 

## LIVE Modeling Workflow
<img width="1173" alt="Figure 1 " src="https://user-images.githubusercontent.com/77795297/186822301-604ec779-88e0-4421-8b4d-9a9dd3592917.png">

Figure 1.- Latent Interacting Variable Effects (LIVE) Modeling Workflow Multi-Omics Microbiome Data is encoded in a set of Sparse Partial Least Square Models. Then, structured model combines discriminative latent variable per each single-omics sPLS-DA models. Next, significant discriminative and predictive omic features are thresholding by VIP, correlational analysis, and q-values to build meta model networks.

## LIVE Modeling Implementation
LIVE Modeling consists on three sequential workbooks: Data Wrangling, Partial Least Squares and Regression, and use Public available metagenomics and metabolomics data set from IBD patients (Franzosa et al, 2019). 

 ![imagen](https://user-images.githubusercontent.com/77795297/186825535-b14d41ca-8640-4822-932b-da16ca7456ea.png)

Data set is split between training and validation data set.

 ![Omics-Data ](https://user-images.githubusercontent.com/77795297/186826287-135b49b0-d2b7-40f9-be64-967dfefe177d.png)

Data Wrangling Workbook 1: It preprocessess training and validation data set.

Partial Least Squares Workbook 2: It establishes sparse Partial Least Squares models. 

Regression Workbook 3: It establishes Linear Interaction Effects Model from sPLS-DA Latent Variable Models.

## LIVE Modeling Reduce 1.62 x 10^9 potential multiomic interactions
![Data Flow](https://user-images.githubusercontent.com/77795297/186826066-f5f59523-8c9c-4825-9c03-f01c1b265ff0.png)

LIVE Modeling FrameworK: doi: https://doi.org/10.1101/2022.07.08.499280 
