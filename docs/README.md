

# docs

Last update: 2024-12-15

This directory contains the `pre-print` and `submissions` directories.

    .
    ├── README.md
    ├── README.qmd
    ├── pre-print
    │   ├── 20231222.docx
    │   ├── 20231222.pdf
    │   ├── 20231223.docx
    │   └── 20231223.pdf
    └── submissions
        ├── 20231222_v1
        │   ├── fig-dissemination-cycle.png
        │   ├── fig-os-flow.png
        │   ├── main_document.pdf
        │   └── title_page.docx
        └── 20240509_r1
            ├── editor_comments.txt
            ├── main.Rmd
            ├── main.log
            ├── main.pdf
            ├── reviewer_1.Rmd
            ├── reviewer_1.pdf
            ├── reviewer_2.Rmd
            ├── reviewer_2.pdf
            ├── reviewer_3.Rmd
            └── reviewer_3.txt

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
