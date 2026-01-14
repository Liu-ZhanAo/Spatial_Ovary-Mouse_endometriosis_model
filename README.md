# Spatial_Ovary-Mouse_endometriosis_model
For analyzing ovarian sections from endometriosis model mice ( Spatial transcriptomic )Spatial transcriptomic

This resource provides a complete set of R scripts for spatial transcriptomic analysis of ovarian tissue sections from a mouse model of endometriosis. The analytical pipeline is organized into six core modules:

Module 1: Cell Type Annotation and Tissue-of-Origin Assignment
Cell types and their tissue origins are identified and validated using spatial transcriptomics data across all samples.

Module 2: Spatial Mapping of Cell Types
Annotated cell type information is overlaid onto the original spatial images of ovarian sections to visualize the spatial distribution of distinct cell populations.

Module 3: Grid-Based Spatial Segmentation Using Signature Cells
The ovarian section is partitioned into regular grid cells. Each grid cell is automatically classified as either normal ovarian tissue or an endometriotic lesion on the ovarian surface, based on the presence or absence of predefined signature cell types within it.

Module 4: Validation Against Pathologist-Defined Ground Truth
The computationally derived segmentation (from Module 3) is quantitatively compared with manual annotations provided by a pathologist to assess concordance and validate the accuracy of the automated approach.

Module 5: Inter-Tissue Heterogeneity Analysis
Systematic comparisons are performed between ovarian tissue and endometriotic lesions with respect to cellular composition and gene expression profiles, revealing distinct molecular and microenvironmental characteristics.

Module 6: Distance-Dependent Transcriptomic Analysis
For a specified cell type of interest, Euclidean distances are computed from each target cell to the nearest cell of the reference type. The relationship between these spatial distances and the expression levels of selected genes in target cells is then analyzed to infer potential distance-dependent regulatory effects.

Requirements: An R environment is required to run the scripts.
Validated Configuration:
R.version
platform x86_64-w64-mingw32
arch x86_64
os mingw32
crt ucrt
system x86_64, mingw32
major 4
minor 4.3
year 2025
month 02
day 28
svn rev 87843
language R
version.string R version 4.4.3 (2025-02-28 ucrt)
nickname Trophy Case
This version uses precise scientific terminology, maintains logical flow, and adheres to conventions common in methods sections of computational biology or spatial omics publications.
