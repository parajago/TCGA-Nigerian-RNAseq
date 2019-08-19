# TCGA-Nigerian-RNAseq

Readme:
This repository contains all of the project code for parsing RNA-seq data and differential expression between Nigerian and TCGA patients.

Aim: To identify unique population-specific genomic drivers and subclone expression patterns using RNAseq data from Nigerian and TCGA breast cancer patients

Considered analyses: 
*Allele-specific expression for specific SNVs, copy number variations or indels identified as different
*ASE Read Counter -> --countOverlapReadsType COUNT_FRAGMENTS (so that it doesn't count fragment overlap at paired read sites) / known or predicted from CGI only (we can manipulate (keep CGI result in the VCF INFO field) and convert CGI tsv file back to single-subject VCF (two samples actually, a T/N pair).)
*Subclonal expression: Correlation to finalized life history anaylsis with DriverNet or BayCount
*Presence of signature switching (within Nigerian group) // HRD
*Early vs late drivers or signatures (within Nigerian group) -> Temporal evolution of signatures
*Immunogenomics expression? / HLA LOH

Folders:
-Code: DESeq2/Limma-voom
-Output: Differential expression analysis tables  
-Plots: Visualization of RNAseq data (batch effect and differential expression)

Workflow:
Phenotype data / inputs saved on UChicago Box and Beagle
Alignment performed with STAR and raw counts generated with HTSeq
DESeq2 for differential analysis
WorkflowR to publish analyses / as lab notebook 

[workflowr]: https://github.com/jdblischak/workflowr
