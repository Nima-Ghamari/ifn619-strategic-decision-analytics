# IFN619 – Strategic Decision Analytics (Queensland Funding + Media Topic Modelling)

This repository contains my IFN619 (Data Analytics for Strategic Decision Makers) project. The work analyses Queensland public funding data to produce decision-focused insights and visual reporting, then extends the analysis with text mining on related media coverage to understand how funding topics are discussed.

## Project goals
- Build a clear analytics narrative for decision-makers (question → data → analysis → visualisation → insight).
- Explore trends and patterns in Queensland funding data across time and categories.
- Apply NLP methods to media coverage to identify themes and clusters, and compare them to structured funding patterns.
- Document limitations and ethical considerations (fairness, representation, and interpretation risk).

## What’s inside
- `UA2-Extended-Analyse.ipynb`  
  Main analysis notebook (data preparation, EDA, visualisations, and NLP pipeline).
- `output_file.csv` (optional)  
  Derived/aggregated outputs created by the analysis (no raw article text).

## Methods and tools
### Structured data analytics
- Data cleaning and feature engineering (Pandas)
- Exploratory analysis and interactive visualisation (Plotly)
- Trend and group comparisons to support evidence-based decisions

### Text mining / NLP (media coverage)
- Text preprocessing and vectorisation (TF-IDF)
- Topic modelling (LDA / NMF)
- Clustering (K-Means) and cluster visualisation (PCA)

## Data and licensing note
This repo does **not** include full-text news articles. Raw Guardian Australia article content was collected for analysis but is excluded here to respect copyright and redistribution limits.  
To reproduce the text analysis, use the notebook workflow to rebuild the dataset from source URLs / APIs and store raw text locally (e.g., in a `data/` folder that is ignored by Git).

## How to run (basic)
1. Create a virtual environment (recommended) and install dependencies:
   - `pandas`, `numpy`, `plotly`, `scikit-learn`, `nltk` (and any others imported in the notebook)
2. Open the notebook and run cells top to bottom:
   - `UA2-Extended-Analyse.ipynb`

> Tip: If you run into missing packages, install exactly what the notebook imports.

## Ethics and limitations
- Correlation ≠ causation: funding patterns and media themes should not be treated as causal.
- Representation risk: media coverage can reflect editorial priorities, not real-world need.
- Fairness: findings should be interpreted carefully, especially when comparing regions or groups.

## Author
Nima Ghamari
