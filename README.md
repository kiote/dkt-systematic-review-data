# Supplementary Materials: A Systematic Review of Deep Knowledge Tracing (2015–2025)

**Paper:** A Systematic Review of Deep Knowledge Tracing (2015–2025): Toward Responsible AI for Education  
**Journal:** Artificial Intelligence Review (Springer Nature)  
**Authors:** Ekaterina Krivich, Danial Hooshyar, Gustav Šír, Yeongwook Yang, Merja Bauters, Raija Hämäläinen, Tommi Kärkkäinen

---

## Overview

This repository contains all supplementary data for the systematic review listed above. It includes the complete screening audit trail, inter-rater reliability files, data extraction matrices, per-study quality appraisal scores, and supporting methodology documents. The materials are organized so that each stage of the review process is traceable and independently verifiable.

---

## Repository Structure

```
dkt-systematic-review-data/
│
├── csv/
│   ├── screening/
│   │   ├── final/                        ← merged screening decisions used in the review
│   │   │   ├── Screenings - 1st Screening.csv
│   │   │   └── Screenings - 2nd screening.csv
│   │   │
│   │   └── raw/                          ← individual scorer sheets and blind samples
│   │       ├── 1st_screening_blind_sample.csv
│   │       ├── 1st_screening_ekaterina_scores.csv
│   │       ├── 2nd_screening_blind_for_ekaterina.csv
│   │       ├── 2nd_screening_blind_sample.csv
│   │       ├── 2nd_screening_danial_scores.csv
│   │       └── 2nd_screening_ekaterina_scores.csv
│   │
│   └── extraction/                       ← analysis-ready extraction matrices per RQ
│       ├── information_extraction.csv
│       ├── papers.csv
│       ├── papers_with_categories.csv
│       ├── papers_rq2.csv
│       ├── papers_rq3.csv
│       ├── papers_rq4.csv
│       └── quality_appraisal.csv
│
└── supplements/                          ← methodology and reporting documents (PDF)
    ├── PRISMA_2020_checklist.pdf
    ├── quality_appraisal_supplement.pdf
    ├── search_strategy.pdf
    └── sensitivity_analysis_supplement.pdf
```

---

## `csv/screening/final/` — Final merged screening decisions used in the systematic review

These files contain the consolidated include/exclude decisions agreed upon by the review team after resolving disagreements. They represent the authoritative record of which papers passed each screening stage and feed directly into the PRISMA flow counts reported in the paper.

- **`Screenings - 1st Screening.csv`** — Merged title-and-abstract screening decisions for all candidate records retrieved from the database search. Each row is one record; columns include DOI, title, year, individual scores, and the final agreed decision.
- **`Screenings - 2nd screening.csv`** — Merged full-text screening decisions for all records that advanced from the first screen. Each row is one paper; columns include DOI, title, and the final include/exclude decision with exclusion reason where applicable.

---

## `csv/screening/raw/` — Raw inter-rater reliability files retained for reproducibility and audit

These files are the unmerged, per-scorer worksheets and randomly drawn blind samples used to calculate inter-rater reliability (Cohen's κ) at each screening stage. They are provided so that any reader can independently verify the agreement statistics reported in the paper and inspect individual scoring decisions before consensus was reached.

- **`1st_screening_blind_sample.csv`** — Randomly sampled subset of first-screen records scored independently by both raters to assess inter-rater reliability; contains title, abstract, and per-rater scores side by side.
- **`1st_screening_ekaterina_scores.csv`** — Ekaterina's individual title-and-abstract screening scores prior to consensus resolution; one row per record with a numeric relevance score (0 = exclude, 0.5 = unsure, 1 = include).
- **`2nd_screening_blind_for_ekaterina.csv`** — The subset of full-text papers presented to Ekaterina as a blinded reliability sample in the second screening round; used to compute second-stage κ.
- **`2nd_screening_blind_sample.csv`** — The full blind-sample record set drawn for second-screen inter-rater reliability calculation, including both raters' scores.
- **`2nd_screening_danial_scores.csv`** — Danial's individual full-text screening scores prior to consensus resolution; one row per paper with include/exclude decision and notes.
- **`2nd_screening_ekaterina_scores.csv`** — Ekaterina's individual full-text screening scores prior to consensus resolution; one row per paper with include/exclude decision and notes.

---

## `csv/extraction/` — Analysis-ready extraction matrices organized by research question

These files contain the structured data extracted from all 84 included studies. Each file is keyed to a specific analytical purpose: the master extraction matrix, the model-architecture categorization used across all RQs, research-question-specific subsets, and the quality appraisal scores. These are the direct inputs to the analyses and figures reported in the paper.

- **`information_extraction.csv`** — Master study-by-variable extraction matrix covering all 84 included papers; columns encode study metadata, model architecture, dataset(s) used, evaluation metrics, reported performance, and methodological attributes extracted for all research questions.
- **`papers.csv`** — Full reference list of all 84 included studies with bibliographic metadata (DOI, title, authors, year, venue); serves as the canonical paper inventory cross-referenced by all other extraction files.
- **`papers_with_categories.csv`** — Extends `papers.csv` with model architecture category labels (e.g., RNN-based, Transformer-based, memory-augmented) assigned during extraction; used to produce taxonomy figures in the paper.
- **`papers_rq2.csv`** — RQ2 subset: data quality analysis variables extracted per study, including dataset characteristics, sample sizes, sparsity indicators, and reported data preprocessing decisions.
- **`papers_rq3.csv`** — RQ3 subset: sequential stability analysis variables, including metrics used to evaluate temporal robustness, sequence-length sensitivity, and cross-dataset generalization results.
- **`papers_rq4.csv`** — RQ4 subset: interpretability and explainability variables, including whether studies report attention visualizations, concept-state diagnostics, or other transparency mechanisms.
- **`quality_appraisal.csv`** — Per-study quality appraisal scores on five criteria (QA1–QA5) derived from the appraisal instrument described in `supplements/quality_appraisal_supplement.pdf`; one row per included study.

---

## `supplements/` — Methodology and reporting documents

PDF documents that describe and report the review methodology in full. These accompany the main paper and provide detail beyond what journal word limits allow.

- **`PRISMA_2020_checklist.pdf`** — Completed PRISMA 2020 reporting checklist, mapping each required item to the corresponding section of the paper.
- **`search_strategy.pdf`** — Full database-specific search strings used across all searched databases, including field tags, Boolean operators, and date filters.
- **`quality_appraisal_supplement.pdf`** — Complete per-study quality appraisal table with scores and justifications for all 84 included studies across all five appraisal criteria.
- **`sensitivity_analysis_supplement.pdf`** — Sensitivity analysis results examining the robustness of inclusion decisions and quality thresholds to alternative scoring assumptions.

---

## License

This dataset is released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material for any purpose, provided appropriate credit is given to the authors and the source paper is cited.
I need to complete my QA verification. The previous attempts were truncated at the final verdict table. Let me deliver my complete assessment concisely.

---

## QA VERIFICATION — COMPLETE

### PART 1: File Structure

| Check | Result |
|---|---|
| `csv/screening/raw/` has 6 files | ✅ All 6 present with correct names |
| `csv/screening/final/` has 2 files | ✅ Both present with correct names (including spaces) |
| `csv/extraction/` has 7 files | ✅ All 7 present with correct names |
| Total CSV count: 15 | ✅ Matches original |
| No loose files in flat `csv/` | ✅ Only subfolders remain |
| `supplements/` has 4 PDFs, untouched | ✅ All 4 present |
| Zero files deleted (20 total) | ✅ Confirmed |

### PART 2: README.md Content

| Check | Result |
|---|---|
| (a) Paper citation & author metadata preserved exactly | ✅ |
| (b) ASCII directory tree matches actual file layout | ✅ All 19 files listed, names exact |
| (c) Every subfolder has a purpose statement | ✅ All 4 subfolder sections present |
| (d) Every individual CSV and PDF described | ✅ 15 CSVs + 4 PDFs = 19/19 |
| (e) CC BY 4.0 license section at bottom | ✅ Correct link, final section |

### Bonus improvements over original README
- `papers.csv` — was in repo but undocumented; now described ✅
- `sensitivity_analysis_supplement.pdf` — was in repo but undocumented; now described ✅

---

## VERDICT

**APPROVED**

All 15 CSV files exist in their correct new locations across the three subfolders. No files remain in the flat `csv/` directory. The `supplements/` folder is untouched with all 4 PDFs. Zero files were deleted. The new README.md preserves the original paper citation and author metadata verbatim, contains an accurate ASCII directory tree matching the actual layout, describes every subfolder with a clear purpose statement, lists and describes all 19 individual data files, and ends with the CC BY 4.0 license section. Two previously undocumented files (`papers.csv` and `sensitivity_analysis_supplement.pdf`) are now properly documented, which is an improvement over the original. The reorganization is complete and correct.