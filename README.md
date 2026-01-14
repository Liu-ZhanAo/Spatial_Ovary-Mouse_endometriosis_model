# Spatial_Mouse_endometriosis_ovary_model

This repository provides a complete set of R scripts for spatial transcriptomics data analysis of ovarian sections from a mouse model of endometriosis. 
The entire analytical pipeline is divided into six core modules:

Module 1: Cell Type Annotation and Tissue-of-Origin Identification,  
Based on spatial transcriptomics data, this module identifies and confirms the cell types and their tissue origins in each sample.

Module 2: Spatial Mapping and Visualization of Cell Types,  
Annotated cell type information is overlaid onto the original spatial images of ovarian sections to visualize the spatial distribution of different cell types.

Module 3: Spatial Grid Partitioning Based on Signature Cells,  
The ovarian section is divided into regular grid units. Each grid is automatically classified as either normal ovarian tissue or an endometriotic lesion on the ovarian surface, based on the presence or absence of specific marker cells within the grid.

Module 4: Validation Against Histopathological Gold Standard,  
The automated segmentation results derived from spatial transcriptomics are compared with manually annotated tissue regions by pathologists to evaluate consistency and validate the accuracy of the computational method.

Module 5: Inter-tissue Heterogeneity Analysis,  
Systematic comparisons are performed between ovarian tissue and endometriotic lesions in terms of cellular composition proportions and gene expression profiles, revealing their molecular and cellular microenvironmental characteristics.

Module 6: Distance-Based Transcriptomic Analysis,  
Using specific cell types as centers, Euclidean distances between target cells and the center cells are calculated. This module analyzes how the expression of specific genes in target cells correlates with their spatial distance from the center.

The raw sequencing data must be processed using SeekSpace® Tools to generate M_endo_1_2_4.rds.

SeekSpace® Tools
http://seekspace.seekgene.com/zh/v1.0.0/index.html

Requirements: R environment
(Verified environment configuration)

> R.version
               _                                
platform       x86_64-w64-mingw32               
arch           x86_64                           
os             mingw32                          
crt            ucrt                             
system         x86_64, mingw32                  
status                                          
major          4                                
minor          4.3                              
year           2025                             
month          02                               
day            28                               
svn rev        87843                            
language       R                                
version.string R version 4.4.3 (2025-02-28 ucrt)
nickname       Trophy Case                      
