

# data

Last update: 2024-12-15

This directory contains the `raw` and `tidy` data directories.

    .
    ├── README.md
    ├── README.qmd
    ├── raw
    │   ├── 2024-11-15_registered_reports_raw.csv
    │   ├── 2024-12-12_registered_reports_raw.csv
    │   ├── 2024-12-13_registered_reports_raw.csv
    │   ├── 2024-12-14_registered_reports2_raw.csv
    │   └── 2024-12-14_registered_reports_raw.csv
    └── tidy
        ├── 2024-11-15_registered_reports.csv
        ├── 2024-12-12_registered_reports.csv
        ├── 2024-12-13_registered_reports.csv
        ├── 2024-12-14_registered_reports.csv
        ├── 2024-12-15_preprints_osf.csv
        └── 2024-12-15_preregistrations_osf.csv

## raw

- This directory contains csv files with preprocessed data about
  registered reports pulled from the OSF framework.
- Every time the data are scraped a new version is included
- The files follow the following format:
  - year-month-day_registered_reports
  - followed by either `raw.csv` or `2raw.csv`
  - the latter represents a more updated version of the data set (i.e.,
    it includes more journals), but it is incomplete in that is does not
    contain all of the same columns as `raw.csv`
  - The most up-to-date files are combined, made tidy in `./main.qmd`
    and stored in the `tidy` direectory, e.g.,
    `2024-12-14_registered_reports.csv`

## tidy

- This directory contains all the tidy csv files, which include:
  - x_registered_reports.csv
  - x_preprints_osf.csv
  - x_preregistrations_osf.csv
- Muliple version exist of some of the files, depending on when the data
  were scraped
- The `x` in the file names above represent the date the data were
  obtained (y-m-d format)
