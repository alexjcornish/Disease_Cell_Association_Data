Disease-Cell Type Association Data
==========

Associations between 503 diseases and 73 cell types were identified using three methods:
- Gene set compactness (GSC)
- Gene set overexpression (GSO)
- Text-mining of the PubMed database. 

The GSC and GSO methods are implemented within the [DiseaseCellTypes R-package][1].

Cornish et al. (2015) contains details on these three methods and how the 503 diseases and 73 cell types were selected.


File Descriptions
----------

- **details_cells.tsv**: Details of the 73 cell types tested. File contains the cell type name (NAME, obtained from FANTOM5), the mapped Cell Ontology ID (CL.ID) and the mapped MeSH terms (MESH). 
- **details_diseases.tsv**: Details of the 503 diseases tested. File contains the disease name (NAME, obtained from DisGeNET), the mapped UMLS IDs (UMLS) and the mapped MeSH terms (MESH). 
- **fantom5_replicates.tsv**: Processed FANTOM5 gene expression data without combination of replicates
- **gsc_pvalues.tsv**: P-values computed using the GSC method. 
- **gso_pvalues.tsv**: P-values computed using the GSO method. 
- **text_pvalues.tsv**: P-values computed through text-mining of PubMed using mapped MeSH terms.



References
----------

[Cornish A.J., Filippis I., David A. and Sternberg M.J.E. (2015) Exploring the cellular basis of human disease through a large-scale mapping of deleterious genes to cell types. Genome Medicine, 7:95][2]

[1]: http://alexjcornish.github.io/DiseaseCellTypes/
[2]: http://genomemedicine.com/content/7/1/95