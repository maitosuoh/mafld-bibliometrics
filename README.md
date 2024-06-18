# Bibliometric analysis of MAFLD literature
This repository contains the R code used for the bibliometric analysis of metabolic (dysfunction)-associated fatty liver disease (MAFLD).  
This study aimed to provide an overview of the research in MAFLD from 2020 to late 2023 using publication metrics. 

## Contents
### Data Source
The literature records were downloaded from PubMed, Web of Science, and Scopus using queries for MAFLD on 2023-10-10.  
These original files were not deposited in this repository due to potential copyright infringement against these databases.

### R environment
The exported files from literature databases were loaded into R environment using bibliometrix (https://www.bibliometrix.org/home/).  
The RStudio workspace after this step (`01_import.RData`) was uploaded in this repository for reproducibility.

### R code
The analysis was performed by running the R codes in the following order with R Studio.

`01_import`: importing files exported from using bibiliometrix   
`02_cleaning`: data cleaning for each dataset from the literature database  
`03_merge`: merging datasets and visualisation of flow chart for literature selection  
`04_journal`: analysis of publication counts and journals (**Fig 1**)  
`05_country`: author country analysis and country co-occurence network analysis (**Fig 6**)  
`06_keyword`: author keyword analysis and keyword co-occurence network analysis (**Fig 2**)  
`07_citation`: extracting reference information from records of Web of Science and Scopus  
`08_co-citation`: citation analysis (**Fig 3**) and co-citation network analysis (**Fig 4, 5**)  
`09_flow_chart`: flow chart for literature selection (**Fig S1**)  
`10_supplementary`: other supplementary figures (**Fig S2-S4**)

### How to use
1. Download all R markdown files from `02.cleaning` to `10.supplementary` in the working directory.
2. Create following folders in the working directory and place the necessary files.  
`data`: used to stored the files downloaded from literature databases (will not be used in this repository).  
`figure`: save pdf files for Figures.  
`rdata`: place `01_import.RData`.  
3. Run the code starting from `02.cleaning`, which loads `01_import.RData` in `rdata` folder.
4. Each file saves the current R workspace at the end of the code in `rdata` folder.
5. The next R markdown file loads the previously saved workspace in the beginning.
6. Run all R markdown files until `10.supplementary` to complete the analysis.
7. The figures produced during the analysis will be stored in `figure` folder.

## Notes
The full list of R packages for data analysis and visualisation is described in the Supplementary materials of the paper.
