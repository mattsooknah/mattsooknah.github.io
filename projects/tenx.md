---
layout: project
title: 10X Genomics
---

I have worked at [10X Genomics](http://www.10xgenomics.com) since January 2016. I've worked on a variety of research projects relating to both 3' RNA sequencing and whole genome / exome sequencing using the 10X molecular barcoding platform.

For IP reasons, I cannot provide full details at this time, but here's an overview.

### SCALING SINGLE CELL TRANSCRIPTOMICS

Single-cell RNA sequencing is a powerful way to profile the gene expression of many cells across multiple cell populations in parallel. The 10X instrument allows capture of up to 48000 cells in one instrument run, using a simpler workflow than most existing protocols.The logical next step is to pool even more cells, across multiple instrument and sequencing runs, in order to increase signal and detect even rarer subpopulations.

I’m working on a pipeline for rapid aggregation of multiple 10X analysis runs, correcting for technical effects across different libraries and sequencing runs. Part of the challenge is adapting existing computational methods for dimensionality reduction and clustering of differential expression data, which are designed to handle a few thousand, rather then 100K+ cells.

I’m also developing a tool that leverages unique molecular identifiers (UMIs) to increase signal across multiple sequencing reads deriving from the same cDNA molecule.

### PHASING LONG MOLECULES

The same 10X platform can also be used for DNA sequencing. Instead of single cells, the sample is partitioned into long molecules (up to ~100KB), which are used to produce short reads with a barcode denoting their source molecule. The barcodes allow downstream analyses to reconstruct the molecules, which provide useful long-range information that can disambiguate between homologous regions and enable haplotype phasing across large chunks of chromosomes.

I’ve made significant contributions to the development of [Long Ranger](http://support.10xgenomics.com/genome-exome/software/pipelines/latest/what-is-long-ranger), our pipeline for analyzing 10X genome and exome data, such as a fast method for stitching together haplotype phase blocks. I’ve also worked on a comprehensive analysis of bait set performance for our exome sequencing kit.
