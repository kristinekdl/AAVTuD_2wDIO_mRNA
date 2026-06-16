------------------------------------------------------------------------

editor_options: markdown: wrap: 72 ---

# 2026_AAV-TuD_2wDIOCohort: Bulk mRNA-seq on iWAT of AAV-TuD 2w DIO Cohort

### *Performed by KDL Q1 2026*

### Project description:

Experiments performed on C57/BL6 TAC males at 10 weeks old at the start of AAV injections. AAV-control-TuD and AAV-miR-335-TuD was injected intra-peritoneally. Animals were on chow diet until 4 weeks-post AAV-injection, where the diet was switched to HFD (60% kcal) and continued for a total of 2 weeks.

The following folders contain:

- `data-raw/`: Raw counts matrix.
- `docs/`: R-markdown files.
- `R/`: Scripts needed to run the R-project.
- `meta/`: Meta data.
- `results/`: Results tables from DE analyses. 1. normalized_counts.csv: CSV file with normalized counts of all genes. 2. sig_DEgenes.csv: CSV file with all significant DE genes (padj\<0.05).
- `figures/`: All figures from entire DE analyses.

# Initiating project environment

Package versions for this project have been managed using `renv`.

- `renv/library`: a library that contains all packages currently used by this project.
- `renv.lock`, records enough metadata about every package that it can be re-installed on a new machine.
- `Rprofile`: a file that is run automatically every time you start R (in this project), and renv uses it to configure your R session to use the project library.

```         
# Download and install packages from this project
renv::restore()
```

# Installing project R package dependencies

Dependencies have been managed by using `usethis::use_package("packagename")` through the `DESCRIPTION` file. Installing dependencies is as easy as opening the `2026_AAV-TuD_2wDIOCohort.Rproj` file and running this command in the console:

```         
# install.packages("pak")
pak::pak()
```

You'll need to have remotes installed for this to work.

# Resource

For more information on this folder and file workflow and setup, check out the [prodigenr](https://rostools.github.io/prodigenr) online documentation.
