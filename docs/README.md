

# docs

Last update: 2025-04-10

This directory contains the `pre-print` and `submissions` directories.

    .
    ├── README.md
    ├── README.qmd
    ├── pre-print
    │   ├── 20231222.docx
    │   ├── 20231222.pdf
    │   ├── 20231223.docx
    │   ├── 20231223.pdf
    │   ├── 20241217.docx
    │   └── 20241217.pdf
    ├── proofs
    │   └── LING.2023.0249.R1_Proof_hi.pdf
    └── submissions
        ├── 20231222_v1
        │   ├── fig-dissemination-cycle.png
        │   ├── fig-os-flow.png
        │   ├── main_document.pdf
        │   └── title_page.docx
        ├── 20240509_r1
        │   ├── editor_comments.txt
        │   ├── main.Rmd
        │   ├── main.log
        │   ├── main.pdf
        │   ├── reviewer_1.Rmd
        │   ├── reviewer_1.pdf
        │   ├── reviewer_2.Rmd
        │   ├── reviewer_2.pdf
        │   ├── reviewer_3.Rmd
        │   └── reviewer_3.txt
        ├── 20241217_v2
        │   ├── author_response.pdf
        │   ├── author_response_blind.pdf
        │   ├── fig-credit-1.png
        │   ├── fig-dissemination-cycle.png
        │   ├── fig-os-flow.png
        │   ├── fig-pp-1.png
        │   ├── fig-pr-1.png
        │   ├── main_document.docx
        │   ├── main_document_highlighted_diffs.docx
        │   └── title_page.docx
        └── 20250410_v3
            ├── fig-credit-1.png
            ├── fig-dissemination-cycle.png
            ├── fig-os-flow.png
            ├── fig-pp-1.png
            ├── fig-pr-1.png
            ├── main_document.docx
            └── title_page.docx

## pre-print

- This directory contains the `docx` and `pdf` versions of the
  manuscript
- The numbers represent the day (ymd) the file was uploaded to psyarxiv

## submissions

- This directory contains subdirectories that are named based on the
  date and version of the project
- The subdirectories contain submissions (ending in `_vX`) and response
  letters (ending in `_rX`)
  - Submission subdirectories contain the anonymized manuscript, title
    page, and corresponding figures that were uploaded the to journal
    website for each version
  - Response letter subdirectories contain the comments from the editor
    and anonymous reviewers (labelled `reviewer_x.Rmd`), as well as the
    author response (`main.Rmd`)
  - Depending on the guidelines of the journal, response letters and
    reviewer comments may be included in the `.gitignore` file, i.e.,
    they may *not* be publicly available
