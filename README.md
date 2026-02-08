# Systematic Mapping Study on Container-Based Virtualization Technologies

[![LaTeX](https://img.shields.io/badge/Built%20with-LaTeX-008080.svg)](https://www.latex-project.org/)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

## Description

This repository contains the LaTeX manuscript for the paper **"Literature Review on Container-Based Virtualization Technologies"**, a Systematic Mapping Study (SMS) that analyzes 226 primary studies published between 2022 and 2024 on container-based virtualization (CBV) technologies.

The study was submitted to the **Journal of Internet Services and Applications (JISA)**.

## Authors

- **José A. Arias-Pinzón** — Universidad del Quindío
- **Anobis H. Correa-Urbano** — Universidad del Quindío
- **Luis E. Sepúlveda-Rodríguez** — Universidad del Quindío
- **Christian A. Candela-Uribe** — Universidad del Quindío

## Article Summary

Container-based virtualization (CBV) has become a cornerstone of modern IT infrastructure, with technologies such as **Docker** and **Kubernetes** dominating application packaging and orchestration, respectively. Despite the proliferation of research in this domain, no existing secondary study systematically mapped CBV technologies across IT domains and academic dimensions (education, research, and outreach).

### Methodology

An SMS was conducted following the guidelines of Petersen et al. and Kitchenham & Charters, using a hybrid search strategy that combines:

- **Database search**: ACM, IEEE Xplore, Springer, Science Direct, and Taylor & Francis (6,530 initial results).
- **Snowballing**: forward and backward citation and reference analysis.
- **Direct inclusion**: articles previously known by the authors.

Studies were evaluated using three quality indices:

| Index | Description |
|-------|-------------|
| **CVI** (Content Validity Index) | Degree of alignment of the study with the SMS objectives |
| **SCI** (Scientific Citation Index) | Citation-normalized impact relative to publication recency |
| **IRRQ** (Index of Relationship to Research Questions) | Coverage of the study with respect to the research questions |

### Classification

The 226 studies were classified along two axes:

- **11 IT domains**: Software Development, Computational Thinking, Parallel Computing, Data Analysis, Artificial Intelligence, Computer Networks, IT Infrastructure, HPC, Security, Cloud Computing, and Blockchain.
- **3 academic dimensions**: Education, Research, and Outreach.

### Key Findings

| Finding | Details |
|---------|--------|
| Technology concentration | Docker (41.6%) and Kubernetes (29.6%) dominate the landscape |
| Domain imbalance | IT Infrastructure accounts for 75.66% of the corpus |
| Academic fragmentation | Research dominates (83.61%), while Education (11.06%) and Outreach (5.88%) are underrepresented |
| Growth | 118% increase in publications from 2022 to 2024 |
| Research gaps | 6 concrete gaps identified (RG1–RG6) |

### Contributions

1. **Comprehensive and reproducible mapping** of the CBV literature across IT domains and academic dimensions.
2. **Dual-axis taxonomy** linking technologies to IT domains and academic impact.
3. **Identification of 6 research gaps** with concrete future directions, including alternative runtime evaluation, educational impact studies, and supply-chain security.

## Repository Structure

```
├── main.tex                    # Main document
├── refs.bib                    # Bibliographic references
├── sbc2019.cls                 # Journal class (JISA/SBC)
├── sections/
│   ├── introduction.tex        # Section 1: Introduction
│   ├── motivation.tex          # Section 2: Motivation
│   ├── related-works.tex       # Section 3: Related Works
│   ├── analysis-and-discussion.tex  # Section 5: Analysis and Discussion
│   ├── threats-to-validity.tex # Section 6: Threats to Validity
│   ├── conclusions.tex         # Section 7: Conclusions
│   └── review-method/          # Section 4: Review Method
│       ├── 00-review-method.tex
│       ├── 01-planning.tex
│       ├── 02-search-studies.tex
│       ├── 03-quality-assessment.tex
│       ├── 04-data-extraction.tex
│       ├── 05-study-clasification.tex
│       ├── 06-results.tex
│       └── 07-reproducibility.tex
├── figures/                    # Figures generated with TikZ/pgfplots
├── resources/images/           # Article images
│   ├── planeacion/
│   ├── busqueda-estudios/
│   ├── resultados/
│   └── taxonomy/
└── README.md
```

## Building

The document uses **XeLaTeX** and **BibTeX**. To compile:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

Or with `latexmk`:

```bash
latexmk -xelatex main.tex
```

### LaTeX Dependencies

The manuscript requires the following packages (included in full TeX Live or MiKTeX distributions):

`fontspec`, `graphicx`, `booktabs`, `tabularx`, `longtable`, `multirow`, `multicol`, `hyperref`, `ragged2e`, `float`, `caption`, `pifont`, `enumitem`, `array`, `adjustbox`, among others.

## Keywords

Container-based virtualization, Systematic mapping study, Docker, Kubernetes, Cloud computing, Software engineering

## License

This work is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).
