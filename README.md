# Bibliometric analysis of MAFLD
This repository contains the code used for the bibliometric analysis of metabolic (dysfunction)-associated fatty liver disease (MAFLD).  
The goal of this study is to provide an overview of the research in MAFLD from 2020 to late 2023 using publication metrics.  
This paper is submitted to a journal and currently under review.

## Contents
### Data Source
The literature records were downloaded from PubMed, Web of Science, and Scopus using queries for MAFLD.
These original files were not deposited in this repository due to potential copyright infringement from these databases.

### Environment
The 
However, the RStudio workspace after loading those files were 

### R code
The whole analysis was 
Each file saves the RStudio workspace at the end of the 

1. import: importing data into  from 
2. cleaning: data cleaning for each 
3. merge: merging datasets and visualisation of flow chart for literature selection (Fig 1)
4. journal: analysis of publication counts and journals(Fig 2)
5. country: author country analysis and country co-occurence network analysis (Fig 7, 8)
6. keyword: author keyword analysis and keyword co-occurence network analysis (Figure 3)
7. citation: extracting reference information from records of Web of Science and Scopus
8. co-citation: citation analysis (Fig 4) and co-citation network analysis (Fig 5, 6)

## Acknowledgements
The data analysis and visualisation was heavily dependent on the  
Hierarchial edge bundling was  (https://r-graph-gallery.com/hierarchical-edge-bundling.html)
The full list of packages are described in the supplementary material of the paper.
