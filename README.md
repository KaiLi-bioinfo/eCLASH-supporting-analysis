# eCLASH: Supporting Analysis of Small RNA-seq and LACE-seq Data

This repository contains scripts for processing MIWI-associated small RNA-seq data.

Small RNA-seq

Reads are adapter-trimmed and collapsed into unique sequences with read counts. Known small RNAs (rRNA, tRNA, snoRNA, snRNA and miRNA) are identified using Bowtie2 and RNAcentral references. Sequences are then aligned to a mouse genome reference. The included summary script reports read lengths and nucleotide preferences (1U).


Scripts

* small_rna/run.sh — small RNA-seq preprocessing and alignment
* small_rna/summary.py — basic small RNA summaries
* config.example.env — reference paths and settings
* environment.yml — software dependencies

Note: These scripts were reorganized from the analysis steps provided for the project. They are not a complete copy of the original analysis pipeline; additional piRNA QC and IgG-background filtering steps are not included. Reference settings should be checked against the data being analyzed.
