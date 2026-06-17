# Single-cell characterization of T-cell exhaustion and macrophage remodeling during LUAD progression and brain metastasis

## Overview

This project investigates immune microenvironment remodeling during lung adenocarcinoma (LUAD) progression and brain metastasis formation using single-cell RNA sequencing (scRNA-seq).

Using publicly available datasets, we analyzed changes in T-cell states, macrophage populations, immune checkpoint expression, and exhaustion-associated transcriptional programs across disease progression.

---

## Study Highlights

### Key findings

- Progressive depletion of cytotoxic CD8+ T cells during tumor progression.
- Expansion of exhausted CD8+ T cells and regulatory T cells (Tregs).
- Replacement of alveolar macrophages by monocyte-derived macrophages.
- Increased expression of immune checkpoint genes:
  - PDCD1 (PD-1)
  - CTLA4
  - LAG3
  - TIGIT
  - HAVCR2 (TIM-3)
  - TOX
- Brain metastases exhibit the strongest immune exhaustion phenotype.

---

## Datasets

### GSE131907

Main discovery cohort:

- 208,506 single cells
- 58 samples
- 44 LUAD patients

Sample types:

- Normal lung tissue (nLung)
- Primary tumors (tLung)
- Brain metastases (mBrain)
- Normal lymph nodes
- Metastatic lymph nodes
- Pleural effusions

### GSE99254

Independent validation cohort used to confirm exhaustion-associated transcriptional programs.

---

## Workflow

1. Data acquisition from GEO
2. Cell annotation integration
3. Immune cell composition analysis
4. T-cell subtype characterization
5. Macrophage remodeling analysis
6. Exhaustion marker analysis
7. Exhaustion score calculation
8. Statistical testing
9. Independent validation
10. Clinical relevance assessment

---

## Repository Structure

```text
luad-brain-metastasis-scRNAseq/

├── GSE131907/
│   ├── figures/
│   ├── manuscripts/
│   ├── processed/
│   ├── raw/
│   └── results/
│
├── GSE99254/
│   ├── figures/
│   ├── manuscripts/
│   ├── processed/
│   ├── raw/
│   └── results/
│
└── README.md
```

---

## Main Figures

## Figures

### GSE131907

- Figure 1 – Cellular composition during LUAD progression
- Figure 2 – T-cell escape and immune remodeling
- Figure 3 – Macrophage remodeling
- Figure 4 – Exhaustion marker heatmap
- Figure 5 – Exhaustion marker expression
- Figure 6A – Exhaustion markers
- Figure 6B – Progressive exhaustion
- Figure 7 – Exhaustion score analysis
- Figure 8 – Exhaustion progression
- Figure 9 – Exhaustion marker dynamics
- Figure 10 – Integrated immune remodeling

### GSE99254 Validation

- Figure 11 – Validation of exhaustion-associated markers in an independent NSCLC cohort
---

## Technologies

- Python 3.13
- pandas
- NumPy
- SciPy
- Matplotlib

---

## Biological Conclusions

Our results indicate that LUAD progression is accompanied by coordinated remodeling of both lymphoid and myeloid compartments. Brain metastases are characterized by profound immune dysfunction, accumulation of exhausted CD8+ T cells, expansion of regulatory T cells, and enrichment of monocyte-derived macrophages, creating a highly immunosuppressive metastatic niche.

---

## Citation

If you use this repository, please cite:

Gabara A. Single-cell characterization of T-cell exhaustion and macrophage remodeling during LUAD progression and brain metastasis.
