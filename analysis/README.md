# TCGA-Nigerian-RNAseq

Readme:
This repository contains all of the project data for parsing RNA-seq data and differential expression between Nigerian and TCGA patients.

Aim: To identify unique population-specific transcriptomic differences using RNAseq data from Nigerian and TCGA breast cancer patients

ANALYSIS:
DESeq2-PC2: Experiments to justify the use of DeSeq2 for within-Nigerian cohort analysis and limma-voom with quantile normalization for Nigerian-TCGA across-cohort analyses in which batch effect is an issue
 
Protein coding-IHC: Supplementary information to the “Life History” project in which samples have been assessed by TP53 and GATA3 mutation status as well as other subgroups involved in the evolutionary development of these tumors. Differential expression analyses within Nigerian or TCGA groups based on mutation status.

PAM50: Differential gene expression stratified by breast cancer subtype between Nigerians and TCGA patients. 

LNC: Long-noncoding RNA analysis (tentative)


CODE: (Supplementary)
TCGA-JSON-parser-2: Code to translate deprecated naming of TCGA samples to modern convention based on JSON file from GDC.

Protein coding parse: Sort whole RNA files into protein-coding, long non-coding or otherwise. 


[workflowr]: https://github.com/jdblischak/workflowr
