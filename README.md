

# Guide to Open Science in Linguistics

Opening open science to all: Demystifying reproducibility and
transparency practices in linguistic research

Preprint: <https://doi.org/10.31234/osf.io/spz4w>  
FOSIL website: <https://fosil-project.github.io>  
RStudio server instance via CodeOcean:
<https://codeocean.com/capsule/2385779/tree>

Last update: 2025-04-17

**Important info**

- Word limit: 8000
- Format: APA
- First submission: 2023-12-22
- Round 1 reviews received: 2024-05-09
- Second submission: 2024-12-17
- Accepted: 2025-04-06

``` r
fs::dir_tree()
```

    .
    ├── README.md
    ├── README.qmd
    ├── README.rmarkdown
    ├── bib
    │   ├── README.md
    │   ├── README.qmd
    │   ├── apa-6th-edition.csl
    │   └── os_refs.bib
    ├── build_qmd.sh
    ├── data
    │   ├── README.md
    │   ├── README.qmd
    │   ├── raw
    │   │   ├── 2024-12-14_registered_reports2_raw.csv
    │   │   ├── 2024-12-14_registered_reports_raw.csv
    │   │   ├── 2025-04-10_registered_reports2_raw.csv
    │   │   └── 2025-04-10_registered_reports_raw.csv
    │   └── tidy
    │       ├── 2024-12-14_registered_reports.csv
    │       ├── 2024-12-15_preprints_osf.csv
    │       ├── 2024-12-15_preregistrations_osf.csv
    │       ├── 2025-04-10_preprints_osf.csv
    │       ├── 2025-04-10_preregistrations_osf.csv
    │       └── 2025-04-10_registered_reports.csv
    ├── docs
    │   ├── README.md
    │   ├── README.qmd
    │   ├── pre-print
    │   │   ├── 20231222.docx
    │   │   ├── 20231222.pdf
    │   │   ├── 20231223.docx
    │   │   ├── 20231223.pdf
    │   │   ├── 20241217.docx
    │   │   └── 20241217.pdf
    │   ├── proofs
    │   │   ├── Attached standard file_ main_document[CE][2025-04-11].docx
    │   │   └── LING.2023.0249.R1_Proof_hi.pdf
    │   └── submissions
    │       ├── 20231222_v1
    │       │   ├── fig-dissemination-cycle.png
    │       │   ├── fig-os-flow.png
    │       │   ├── main_document.pdf
    │       │   └── title_page.docx
    │       ├── 20240509_r1
    │       │   ├── editor_comments.txt
    │       │   ├── main.Rmd
    │       │   ├── main.log
    │       │   ├── main.pdf
    │       │   ├── reviewer_1.Rmd
    │       │   ├── reviewer_1.pdf
    │       │   ├── reviewer_2.Rmd
    │       │   ├── reviewer_2.pdf
    │       │   ├── reviewer_3.Rmd
    │       │   └── reviewer_3.txt
    │       ├── 20241217_v2
    │       │   ├── author_response.pdf
    │       │   ├── author_response_blind.pdf
    │       │   ├── fig-credit-1.png
    │       │   ├── fig-dissemination-cycle.png
    │       │   ├── fig-os-flow.png
    │       │   ├── fig-pp-1.png
    │       │   ├── fig-pr-1.png
    │       │   ├── main_document.docx
    │       │   ├── main_document_highlighted_diffs.docx
    │       │   └── title_page.docx
    │       └── 20250410_v3
    │           ├── fig-credit-1.png
    │           ├── fig-dissemination-cycle.png
    │           ├── fig-os-flow.png
    │           ├── fig-pp-1.png
    │           ├── fig-pr-1.png
    │           ├── main_document.docx
    │           └── title_page.docx
    ├── figs
    │   ├── README.md
    │   ├── README.qmd
    │   ├── credit
    │   │   ├── fig-credit-1.pdf
    │   │   └── fig-credit-1.png
    │   ├── dissemination-cycle
    │   │   ├── fig-dissemination-cycle-theme
    │   │   ├── fig-dissemination-cycle.mmd
    │   │   ├── fig-dissemination-cycle.png
    │   │   └── fig-dissemination-cycle.psd
    │   ├── os-flow
    │   │   ├── fig-os-flow.mmd
    │   │   ├── fig-os-flow.png
    │   │   └── fig-os-flow.psd
    │   ├── preprints
    │   │   ├── fig-pp-1.pdf
    │   │   └── fig-pp-1.png
    │   └── preregistration
    │       ├── fig-pr-1.pdf
    │       └── fig-pr-1.png
    ├── guide_to_open_science.Rproj
    ├── main.docx
    ├── main.qmd
    ├── ref_doc
    │   ├── README.md
    │   ├── README.qmd
    │   └── apa_style.docx
    └── tables
        ├── README.md
        ├── README.qmd
        ├── platform_features.csv
        ├── preprint_servers.csv
        ├── rr_journals.csv
        └── table_draft.docx
