
## Abstract

Expression omics data can be analysed for differential expression with respect to biological conditions like disease status. An intuitive method to understand the functional implication of differential expression is pathway analysis. Pathways are networks of interacting biomolecules and represent discrete biological functions. Current methods of pathway analysis are based on the relative difference in expression of either genes or metabolites between biological states. These methods are classified as over-representation and functional class scoring. A widely used method is gene set enrichment analysis. This analysis when, applied to metabolites is called metabolite set enrichment analysis. The three main drawbacks of these methods are, first, they are unable to quantify differential pathway regulation at a sample level as they are based on summary statistics (for example, mean). It is not possible to explore individual biological variation between samples. Second, they assume equal contribution of biomolecular expression to pathway regulation. Third, they have not been applied in the analysis of integrated expression data. A method to perform personal pathway analysis using concatenated multi-omics expression data was developed to address these shortcomings. Co-variance of molecules in each pathway was modelled by factor analysis with one factor representing the pathway. Factor scores obtained, quantified pathway regulation at the sample level. The contribution of each molecule to pathway regulation was quantified by the loadings. The method was used to analyse transcriptomic and metabolomic expression of skeletal muscle tissue from a type II diabetes (T2D) study. Differential pathway regulation analysis was performed using quantified pathway regulation values and relevant clinical variables. The analysis identified several differentially regulated pathways that are linked to T2D pathology of skeletal muscle tissue. These included Defects in biotin (Btn) metabolism and Branched-chain amino acid catabolism, among others. Results were compared with IMPaLA, which is a tool for p-value integration of gene and metabolite set enrichment analyses. Dynamic visualisation dashboards (using bokeh in python) were developed to explore biological heterogeneity of individuals’ pathway regulation and contribution of biomolecules to pathway regulation. This analysis advances personalised omics research and can potentially be adapted to analysis of single cell expression.

## Dashboards

Dynamic dashboards exploring pathway regulation in context of the following clinical variables were developed using the bokeh package in python. [Online viewer](https://htmlpreview.github.io/)

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

(C) Revant Gupta (2018). "Personal pathway analysis as a means to integrate metabolomic and transcriptomic data in T2D intervention studies". Master's thesis for Molecular Techniques in Life Science. KTH Royal Institute of Technology, Karolinska Institutet, Stockholm University, and Science for Life Laboratory.
