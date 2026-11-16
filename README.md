A4549 RNA-seq Analysis: Sodium Propionate Treatment 

1. Project Overview
This project investigates gene expression changes in A549 lung cancer cells following three days of sodşum propionate treatment. The analysis focuses on differential gene expression and 
Hallmark pathway enrichment, particularly pathways associated with epithelial identity.

The RNA-seq dataset was obtained from NCBI GEO (GSE224740)

2.Dataset 
The dataset includes six biological samples: 
 -Control(3 replicates)
 -Sodium Propionate-treated (3 replicates)

3.Analysis Workflow 
 -Import raw RNA-seq counts and construct a SummarizedExperiment object.
 -Filter low-expression genes and examine sample variation using PCA
 -Perform differential expression analysis using DESeq2.
 -Perform preranked gene-set enrichment analysis using fgsea and human MsigDB Hallmark gene sets (Version 2026.1.Hs)
 -Examine leading-edge genes fram EMT, Apical Junction and Apical Surface pathways.
 -Visualize 15 selected leading-edge genes using a heatmap.
 
 4.How To Reproduce the Analysis
  -Install R and Rstudio.
  -Clone or download this repository.
  -Open Task6_A549.Rproj in Rsudio.
  -Restore the required packages using renv::restore()
  -Open task6_A549.Rmd and click Knit to generate HTML report
  
  5.Data Source
  https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE224740 

