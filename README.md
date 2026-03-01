# KICH-RNAseq-analysis

## Introduction 

## Overview
Differential expression analysis of kidney chromophobe cancer (KICH) 
tumor vs. normal tissue using bulk RNA-seq data from TCGA.

## Data 
Downloaded from UCSC Xena (GDC Hub):
- Gene expression: STAR - Counts (n=91): https://xenabrowser.net/datapages/?dataset=TCGA-KICH.star_counts.tsv&host=https%3A%2F%2Fgdc.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

- Clinical metadata: Phenotypes (n=91): https://xenabrowser.net/datapages/?dataset=TCGA.KICH.sampleMap%2FKICH_clinicalMatrix&host=https%3A%2F%2Ftcga.xenahubs.net&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443

## Methods
- Differential expression: DESeq2
- Visualization: volcano plot, heatmap
- Pathway enrichment: clusterProfiler

## How to reproduce
1. Download data from UCSC Xena links above
2. Place files in `data/`
3. Run `notebooks/analysis.Rmd`

## Requirements
R packages: DESeq2, clusterProfiler, tidyverse, pheatmap, ggrepel