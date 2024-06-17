# Bibliometric analysis of MAFLD literature
This repository contains the R code used for the bibliometric analysis of metabolic (dysfunction)-associated fatty liver disease (MAFLD).  
This study aimed to provide an overview of the research in MAFLD from 2020 to late 2023 using publication metrics.  
The manuscript is submitted to a journal and currently under review.

## Contents
### Data Source
The literature records were downloaded from PubMed, Web of Science, and Scopus using queries for MAFLD on 2023-10-10.  
These original files were not deposited in this repository due to potential copyright infringement against these databases.

### R environment
The exported files from literature databases were loaded into R environment using bibliometrix (https://www.bibliometrix.org/home/).  
The RStudio workspace after this step (`01_import.RData`) was uploaded in this repository for reproducibility.

### R code
The analysis was performed by running the R codes in the following order with R Studio.

`01. import`: importing files exported from using bibiliometrix   
`02. cleaning`: data cleaning for each dataset from the literature database  
`03. merge`: merging datasets and visualisation of flow chart for literature selection (Fig 1)  
`04. journal`: analysis of publication counts and journals(Fig 2)  
`05. country`: author country analysis and country co-occurence network analysis (Fig 7, 8)  
`06. keyword`: author keyword analysis and keyword co-occurence network analysis (Figure 3)  
`07. citation`: extracting reference information from records of Web of Science and Scopus  
`08. co-citation`: citation analysis (Fig 4) and co-citation network analysis (Fig 5, 6) 
`09. flow chart`: flow chart for literature selection (Fig S1)  
`10. supplementary`: other supplementary figures (Fig S2-S4)

### How to use
Download and place the R workspace and all R code files from 2. cleaning in your working directory.
Open 2. cleaning with RStudio and run the code, which will start by loading the deposited workspace.
Each Figure in the paper will be saved as a single pdf file.
Each file saves the current R workspace at the end, and the next file loads the generated workspace in the beginning. 
(Because the original record files exported from the literature databases are not provided, the code in 1_import does not work)

### Session info

## Acknowledgements
The full list of R packages for data analysis and visualisation is described in the supplementary material of the paper.
