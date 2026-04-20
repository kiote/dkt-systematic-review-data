# Supplementary Data: A Systematic Review of Deep Knowledge Tracing (2015–2025)

**Paper:** A Systematic Review of Deep Knowledge Tracing (2015–2025): Toward Responsible AI for Education  
**Journal:** Artificial Intelligence Review (Springer Nature)  
**Authors:** Ekaterina Krivich, Danial Hooshyar, Gustav Šír, Yeongwook Yang, Merja Bauters, Raija Hämäläinen, Tommi Kärkkäinen

---

## Overview

This repository contains the data extraction and supplementary materials for the systematic review listed above.

---

## Repository Structure

```
├── csv/
│   ├── information_extraction.csv    ← Final data extraction for all 84 included studies
│   └── quality_appraisal.csv         ← Per-study quality appraisal scores
│
└── supplements/
    ├── PRISMA_2020_checklist.pdf      ← PRISMA 2020 checklist (Supplementary Material D)
    ├── search_strategy.pdf            ← Database-specific search queries (Supplementary Material A)
    ├── quality_appraisal_supplement.pdf ← Per-study quality appraisal detail (Supplementary Material B)
    └── sensitivity_analysis_supplement.pdf ← Sensitivity analysis (Supplementary Material C)
```

---

## Data Extraction (`csv/information_extraction.csv`)

The main data file contains one row per included study (N = 84) with the following columns:

| Column | Description |
|--------|-------------|
| ID | Study identifier (1–84) |
| DOI | Digital Object Identifier |
| Year | Publication year |
| Title | Paper title |
| Authors | Author list |
| Country | Country of first author's affiliation |
| Publication Type | Conference or journal |
| Publication Venue | Name of journal or conference proceedings |
| Keywords | Author-provided keywords |
| Objectives | Study objectives |
| Ethical Concerns | Any ethical framework discussion in the paper |
| Underlying Theories | Theoretical foundations cited |
| Method | Algorithms and model architecture |
| Dataset | Datasets used, including sample sizes |
| Field of Study | Educational domain (e.g., Math, Programming) |
| Input Features | Input representation description |
| Validation Method | Evaluation protocol (e.g., 5-fold cross-validation) |
| Metrics | Reported evaluation metrics |
| RQ2: Data Quality | Whether and how the study addresses data quality issues |
| RQ3: Sequential Stability | Whether and how the study addresses sequential stability |
| RQ4: Interpretability | Whether and how the study addresses interpretability |
| Limitations | Study-reported limitations |
| Challenges and Future Directions | Study-reported future work |

## Quality Appraisal (`csv/quality_appraisal.csv`)

Per-study quality appraisal scores across five criteria, as described in the manuscript (Section 2.4).

---

## License

This data is provided to support the reproducibility of the systematic review. Please cite the paper if you reuse it.
