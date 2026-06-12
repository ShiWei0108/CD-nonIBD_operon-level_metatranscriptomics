# CD-nonIBD_operon-level_metatranscriptomics
Operon-level metatranscriptomic analysis of CD vs non-IBD gut microbiome: from read processing to KEGG enrichment and ReporterScore. Includes custom operon prediction, Salmon quantification, DESeq2, eggNOG-mapper, hypergeometric test, and ReporterScore.

This repository contains all code and workflows for the operon‑centric analysis of metatranscriptomic data comparing Crohn’s disease (CD) and non‑inflammatory bowel disease (non‑IBD) gut microbiomes.

## Key features

- **Operon prediction**: custom Python script (same contig, same strand, intergenic gap <50 bp)
- **Quantification**: Salmon with operson reference library
- **Differential expression**: DESeq2 (|log2FC|>1, padj<0.05)
- **Functional annotation**: eggNOG‑mapper (KO, KEGG pathways)
- **Enrichment analyses**:
  - Hypergeometric test on significantly expressed genes
  - ReporterScore (GRSA) on full KO abundance matrix
- **Visualisation**: bubble plots, bar plots, volcano plots
