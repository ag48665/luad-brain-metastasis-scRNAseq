# Single-cell characterization of T-cell exhaustion and macrophage remodeling during LUAD progression and brain metastasis

## Overview

This repository contains a comprehensive single-cell RNA sequencing (scRNA-seq) analysis investigating immune microenvironment remodeling during lung adenocarcinoma (LUAD) progression and brain metastasis formation.

The study focuses on identifying cellular and transcriptional mechanisms associated with metastatic progression, immune escape, T-cell exhaustion, and macrophage remodeling. Using publicly available datasets, we characterized changes in immune cell composition and exhaustion-associated programs across different stages of disease progression.

---

## Scientific Motivation

Brain metastases represent one of the most severe complications of lung adenocarcinoma (LUAD), occurring in approximately 20–40% of patients during disease progression. Despite advances in targeted therapies and immune checkpoint inhibitors, prognosis remains poor once metastatic spread to the central nervous system occurs.

The biological mechanisms driving immune dysfunction during metastatic progression remain incompletely understood. Single-cell transcriptomics provides an opportunity to dissect the tumor microenvironment at cellular resolution and identify immune cell populations contributing to disease progression and therapeutic resistance.

This project aims to characterize these processes and identify exhaustion-associated transcriptional programs that may represent future therapeutic targets.

---

## Study Highlights

### Key Findings

* Progressive depletion of cytotoxic CD8+ T cells during LUAD progression.
* Expansion of exhausted CD8+ T cells and regulatory T cells (Tregs).
* Replacement of tissue-resident alveolar macrophages by monocyte-derived macrophages.
* Increased expression of immune checkpoint molecules:

  * PDCD1 (PD-1)
  * CTLA4
  * LAG3
  * TIGIT
  * HAVCR2 (TIM-3)
  * TOX
* Progressive increase in exhaustion scores across disease stages.
* Brain metastases exhibit the strongest immune exhaustion phenotype.
* Independent validation confirms exhaustion-associated transcriptional programs.

---

## Research Questions

This study addresses several key questions:

1. How does immune cell composition change during LUAD progression?
2. Which T-cell populations are preferentially expanded or depleted?
3. How do exhaustion-associated transcriptional programs evolve during metastatic progression?
4. What macrophage populations dominate metastatic lesions?
5. Are exhaustion signatures reproducible in independent patient cohorts?
6. Which immune checkpoint pathways may represent clinically relevant therapeutic targets?

---

## Datasets

### GSE131907 – Discovery Cohort

Main dataset used for hypothesis generation and biological discovery.

Characteristics:

* 208,506 single cells
* 58 samples
* 44 LUAD patients

Sample types:

* Normal lung tissue (nLung)
* Primary tumors (tLung)
* Brain metastases (mBrain)
* Normal lymph nodes
* Metastatic lymph nodes
* Pleural effusions

### GSE99254 – Validation Cohort

Independent NSCLC cohort used to validate exhaustion-associated transcriptional programs identified in the discovery dataset.

---

## Workflow

### Data Processing

1. Data acquisition from GEO
2. Quality assessment
3. Cell annotation integration
4. Immune cell extraction
5. Cell-type abundance analysis

### Biological Analysis

6. T-cell subtype characterization
7. Macrophage remodeling analysis
8. Exhaustion marker profiling
9. Exhaustion score calculation
10. Comparative stage-specific analysis

### Validation

11. Independent cohort validation (GSE99254)
12. Statistical evaluation
13. Biological interpretation

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

## Figures

### Discovery Dataset (GSE131907)

| Figure    | Description                                  |
| --------- | -------------------------------------------- |
| Figure 1  | Cellular composition during LUAD progression |
| Figure 2  | T-cell escape and immune remodeling          |
| Figure 3  | Macrophage remodeling                        |
| Figure 4  | Exhaustion marker heatmap                    |
| Figure 5  | Exhaustion marker expression                 |
| Figure 6A | Exhaustion-associated marker analysis        |
| Figure 6B | Progressive T-cell exhaustion                |
| Figure 7  | Exhaustion score analysis                    |
| Figure 8  | Exhaustion progression                       |
| Figure 9  | Exhaustion marker dynamics                   |
| Figure 10 | Integrated immune remodeling model           |

### Validation Dataset (GSE99254)

| Figure    | Description                                             |
| --------- | ------------------------------------------------------- |
| Figure 11 | Independent validation of exhaustion-associated markers |

---

## Biological Conclusions

Our analysis demonstrates coordinated remodeling of both lymphoid and myeloid compartments during LUAD progression.

Major observations include:

* Progressive loss of functional cytotoxic T-cell populations.
* Expansion of exhausted CD8+ T cells characterized by elevated checkpoint receptor expression.
* Increased abundance of immunosuppressive macrophage populations.
* Establishment of a profoundly dysfunctional immune microenvironment in brain metastases.
* Validation of exhaustion-associated transcriptional programs in an independent NSCLC cohort.

Collectively, these findings suggest that metastatic progression is accompanied by extensive immune dysfunction and may provide opportunities for combination immunotherapeutic strategies targeting both exhausted T cells and macrophage-mediated immunosuppression.

---

## Clinical Relevance

The observed immune remodeling patterns may contribute to:

* Resistance to immune checkpoint blockade.
* Reduced anti-tumor immune surveillance.
* Increased metastatic potential.
* Poor clinical outcomes in advanced LUAD.

Our findings support further investigation of:

* TOX-mediated T-cell dysfunction
* Immune checkpoint co-expression programs
* Macrophage-targeted therapeutic strategies
* Combination immunotherapy approaches

---

## Technologies

Analyses were performed using:

* Python 3.13
* pandas
* NumPy
* SciPy
* Matplotlib

---

## Data Availability

All datasets analyzed in this project are publicly available through the NCBI Gene Expression Omnibus (GEO):

* GSE131907
* GSE99254

No patient-identifiable information is included in this repository.

---

## Limitations

Several limitations should be considered:

* Analyses are based on publicly available datasets.
* Clinical metadata availability is limited.
* Findings are primarily observational.
* Functional validation experiments were not performed.
* Additional independent cohorts are needed for further validation.

---

## Future Directions

Potential future extensions include:

* Integration of additional LUAD brain metastasis datasets.
* Pseudotime analysis of exhaustion trajectories.
* Cell-cell communication analysis.
* Spatial transcriptomics integration.
* Survival modeling using exhaustion-associated signatures.
* Predictive biomarker development for immunotherapy response.

---

## Author

**Agata Gabara**

Bioinformatics | Cancer Genomics | Single-Cell Transcriptomics

---

## Citation

If you use this repository, please cite:

**Gabara A.** Single-cell characterization of T-cell exhaustion and macrophage remodeling during LUAD progression and brain metastasis.

---

## License

This repository is provided for academic and research purposes.
