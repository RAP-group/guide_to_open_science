

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
- All data sets are loaded from `./main.qmd`

## Data dictionaries

### x_registered_reports.csv

- The original data sets is provided by the OSF at
  <https://docs.google.com/spreadsheets/d/1D4_k-8C_UENTRtbPzXfhjEyu3BfLxdOsn9j-otrO870/edit#gid=0>
  and <https://www.cos.io/initiatives/registered-reports>
- The complete data dictionary is provided by the OSF is reproduced here
  for convenience:
  - DEFINITIONS OF FEATURES (Note that Criteria 1 and 2 are the minimal
    necessary conditions to qualify as a Registered Report):
    1.  Includes pre-study peer review: Whether the journal will subject
        the pre-study proposal to peer review. A pre-study proposal is
        one evaluated prior to anyone observing study outcomes – usually
        prior to data collection.
    2.  Offers provisional pre-study acceptance: Whether the journal
        offers ‘in principle acceptance’ of proposals, guaranteeing to
        publish the study regardless of the outcome of the registered
        hypothesis tests. (Note: satisfying this condition does not
        require unconditional acceptance).
    3.  Permanence of adoption: Whether the journal is offering RRs
        indefinitely or instead for a trial period or as part of a
        special issue.
    4.  Offered for novel studies: Whether the journal is offering RRs
        for original studies.
    5.  Offered for replication studies: Whether the journal offering
        RRs for studies seeking to specifically replicate previous
        research.  
    6.  Offered for meta-analysis: Whether the journal will consider RRs
        that propose meta-analyses.
    7.  Offered for analyses of existing data sets: Whether the journal
        will consider RRs for analysis of data that already exists.
    8.  Publishes Registered Reports only: Whether the journal is
        dedicated solely to publishing Registered Reports.
    9.  Allows reporting of unregistered analyses: Whether the RR format
        allows authors to report unregistered exploratory analyses in
        the final results (appropriately identified).
    10. Includes post-study peer review: Whether the journal offers peer
        review of the completed paper following data collection and
        analysis.
    11. Allows inclusion of unregistered pilot studies: Whether the
        journal allows authors to include the outcomes of completed
        pilot experiments within pre-study proposals.
    12. Requires public data deposition: Whether the journal requires
        authors to publish all relevant data collected as part of the
        research within a freely accessible repository.
    13. Specifies structured criteria for editorial decisions: Whether
        the journal specifies the criteria according to which
        manuscripts will be accepted or rejected at all stages.
    14. Requires submitted protocols to have prior ethical approval:
        Whether the journal requires authors to have obtained formal
        ethical approval to conduct the proposed research prior to
        submission of the pre-study protocol.
    15. Specifies minimum statistical power requirements: Whether the
        journal guidelines state a minimum threshold for statistical
        power of pre-registered statistical tests or alternate
        (e.g. Bayesian) criteria for completion of data collection.
    16. Will publish ‘Withdrawn Registrations’: Whether the journal will
        publish a withdrawn registration (including at a minimum the
        study title, brief study information, and reason for withdrawal)
        if authors voluntarily remove their study from consideration
        following the award of provisional acceptance. (Note: does not
        apply to editorial rejections).
    17. Publishes accepted protocols, in full or part, prior to study
        completion: Whether the journal publishes any part of the
        pre-study protocol prior to acceptance of the final manuscript
        that describes the completed study. This could include anything
        from the title alone to the full study protocol, and could be
        on-line only or in its journal pages.
    18. Offers incremental (sequential) registration: Whether the
        journal gives authors the option of proposing and
        pre-registering follow-up studies following final acceptance of
        a completed study, rather than publishing immediately.
    19. Offers incremental addition of unregistered studies: Whether the
        journal gives authors the option of reporting additional
        unregistered (exploratory) studies following reporting of the
        approved pre-registered research.
    20. Offered for qualitative studies.
    21. Requires deposition of the Stage 1 protocol at the point of IPA
        in a recognised public registry
  - Note: we have added an additional column, `is_ling`, which indicates
    whether or not the journal is related to ‘language’ or ‘linguistics’
    based on the title

### 2024-12-15_preprints_osf.csv

- This data set was scraped from the OSF website
  (<https://osf.io/search?resourceType=Preprint>)
- There are two columns in the original data set, which we have labelled
  `year` and `count`, and an additional column added in post-processing,
  `cumsum`
  - **year**: (numeric) time period for preprint registration
  - **count**: (numeric) number of registrations
  - **cumsum**: (numeric) cumulative sum of counts over time

### 2024-12-15_preregistrations_osf.csv

- This data set was scraped from the OSF website
  (<https://osf.io/search?resourceType=Registration>)
- There are two columns in the original data set, which we have labelled
  `year` and `count`, and an additional column added in post-processing,
  `cumsum`
  - **year**: (numeric) time period for preprint registration
  - **count**: (numeric) number of registrations
  - **cumsum**: (numeric) cumulative sum of counts over time
