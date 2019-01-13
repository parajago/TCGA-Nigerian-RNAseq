Readme:
This repository contains all of the project code for parsing RNA-seq data and differential expression between Nigerian and TCGA patients.

Aim: To identify unique population-specific genomic drivers and subclone expression patterns using RNAseq data from Nigerian and TCGA breast cancer patients

Pending analyses: 
N Comments:
-Check the 14q gene loss across the groups
-Make a volcano plot
-Assess driver candidate genes, subtypes and protein coding genes
-Redo the analysis with whole genome sequencing only

H Comments:
-*Correlate significant genes to function via gencode 26 assuming +/- annotation did not work out and isolate differential expression of protein coding genes

A Comments: 
-Reverse TSNE of the data to understand if any correlative relationships
-Read about cross-validated lasso and GLMnet -> visual outputs (2 hours)

M Comments:
-Redo normalization
-Breast cancer subtypes

*Overall differences in candidate driver gene expression | controlling for subtype
*Allele-specific expression for specific SNVs, copy number variations or indels identified as different
*ASE Read Counter -> --countOverlapReadsType COUNT_FRAGMENTS (so that it doesn't count fragment overlap at paired read sites) / known or predicted from CGI only (we can manipulate (keep CGI result in the VCF INFO field) and convert CGI tsv file back to single-subject VCF (two samples actually, a T/N pair).)
*Subclonal expression: Correlation to finalized life history anaylsis with DriverNet or BayCount
*Presence of signature switching (within Nigerian group) // HRD
*Early vs late drivers or signatures (within Nigerian group) -> Temporal evolution of signatures
*Immunogenomics expression? / HLA LOH



Folders:
-Code: DESeq2
-Output: Differential expression analysis tables  
-Plots: Visualization of RNAseq data (batch effect and differential expression)



Workflow:
Phenotype data / inputs saved on UChicago Box and Beagle
Alignment performed with STAR and raw counts generated with HTSeq
DESeq2 for differential analysis
WorkflowR to publish analyses / as lab notebook 
