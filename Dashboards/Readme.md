
## Abstract

A method to perform personalised pathway analysis using concatenated multi-omics expression data. Pathway definitions from the Reactome database were used to create sets of molecules that included transcripts and metabolites. Co-variance of molecules in each set was modelled using factor analysis with one factor representing the pathway. Factor scores obtained quantified pathway regulation per sample. Contribution of each molecule to the regulation of the pathway was quantified by the loadings. This method addresses several shortcomings of current differential pathway methods based on over- representation and functional class scoring like gene set enrichment analysis. The method was used to analyse data from a type II diabetes study. Results were compared with IMPaLA, a method for integration of transcriptomic and metabolomic set enrichment analyses.

## Dashboards

Dynamic dashboards exploring pathway regulation in context of the following clinical variables were developed using the bokeh package in python.

### Clinical variables

* M-index: The M index is a measure of glycaemic variability and magnitude.
* HbA1c: Glycated haemoglobin.
* HOMA-IR: Homeostatic model assessment-Insulin resistance.
* S. C-peptide: Serum C-peptide.
* F.P. glucose: Fasting plasma glucose.


### Instructions to use the dashboards

* The title of this dashboard is the ANCOVA model. 
* The '!' symbol marks the variable under investigation and the rest are blocking variables. 
* Each circle represents is a pathway. 
* Click on the circle to dynamically update the attached plot. 
* Hover over the circles for details about the pathway.
* The default view on the charts are from the factor analysis model of the entire dataset.
* Relative contributions are loadings scaled to range (1,-1).