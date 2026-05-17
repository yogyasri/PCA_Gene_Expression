# PCA on Gene Expression Data

BEE-102 assignment - reproducing Figure 1 from the Nature PCA primer using breast cancer expression data (GSE5325).

## How to Run

1. Upload `pca.ipynb` to Google Colab (or Jupyter)
2. Upload the `data/` folder with `class.tsv`, `filtered.tsv.gz`, `columns.tsv.gz`
3. Run all cells

Uses numpy, pandas, matplotlib.

## What it does

- Loads expression data for 105 breast cancer patients (ER+ and ER-)
- Plots GATA3 vs XBP1 scatter (panel a)
- Does manual PCA using SVD (not sklearn)
- Generates the 6 panels from Figure 1: original space, PCA vectors, PC1 projection, scree plot, biplot, and multi-class view

## Data

- `data/class.tsv` - patient labels (1=ER+, 0=ER-)
- `data/filtered.tsv.gz` - expression matrix (105 patients x 16174 genes)
- `data/columns.tsv.gz` - gene ID mapping
