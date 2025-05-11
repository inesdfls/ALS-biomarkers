# Post-mortem Gene Analysis: Identification of Links with ALS

## Introduction

This project focuses on identifying potential biomarkers associated with Amyotrophic Lateral Sclerosis (ALS) using RNA-Seq data from post-mortem brain cortex biopsies. ALS is a progressive neurodegenerative disease affecting motor neurons in the brain and spinal cord, leading to muscle weakness, paralysis, and ultimately respiratory failure. The objective of this project is to uncover specific molecular signatures that correlate with ALS pathology, potentially improving our understanding of the disease and guiding future therapeutic strategies.

## Project Structure

The project is divided into several key steps:

### Step 1 – Data Pre-processing

* **Gather RNA Counts**: Extracted RNA counts from the original data files and stored them in a DataFrame named 'data\_matrix', where each row represents a patient and each column represents a gene.
* **Gather Sample Annotations**: Created a separate DataFrame named 'data\_annotation' to store additional patient information, including disease status and sample source, ensuring accurate data linkage.

### Step 2 – Descriptive Analysis

* **Sample Description**: Analyzed the distribution of samples based on disease group and CNS subregions.
* **RNA Counts Description**: Identified the top 10 genes with the highest and lowest mean expression levels.

### Step 3 – PCA (Principal Component Analysis)

* Conducted PCA to reduce the dimensionality of the data and visualize potential groupings based on disease status and CNS subregion.

### Step 4 – Univariate Analysis

* Used pydeseq2 to identify significantly differentially expressed genes.

### Step 5 – Multivariate Analysis

* Applied Elastic-Net to identify the top 100 candidate genes potentially associated with ALS.

## Key Findings

* Some genes with the highest and lowest mean expressions are potentially linked to ALS.
* PCA did not reveal clear groupings based on disease status or CNS subregion.
* Identified 100 candidate genes likely associated with ALS through multivariate analysis.

## Challenges

* Managing time effectively with other academic commitments.
* Ensuring accurate data processing and annotation.

## Conclusion

This project provided valuable insights into ALS-related biomarkers and enhanced our understanding of bioinformatics techniques, including data pre-processing, PCA, and multivariate analysis. It also highlighted the importance of data quality and careful analysis in biomedical research.

## Authors

* **Nourchen Marzouki** - University Paris-Saclay, UFR Sciences
* **Inès Duflos** - University Paris-Saclay, UFR Sciences
