Disease-Cell Type Association Data
==========

The disease-cell type association data computed using the [DiseaseCellTypes R-package][1] and text-mining of PubMed.

Associations between 503 diseases and 73 cell types are identified using three methods:
- Gene set compactness (GSC)
- Gene set overexpression (GSO)
- Text-mining of the PubMed database. 

Cornish et al. (2015) contains details on these three methods and how thr 503 diseases and 73 cell types were selected.


File Descriptions
----------

- **details_cells.tsv**: Matrix of details of the 73 cell types tested. File contains the cell type name (NAME, obtained from FANTOM5), the mapped Cell Ontology ID (CL.ID) and the mapped MeSH terms (MESH). 
- **details_diseases.tsv**: Matrix of details of the 503 diseases tested. File contains the disease name (NAME, obtained from DisGeNET), the mapped UMLS IDs (UMLS) and the mapped MeSH terms (MESH). 
- **gsc_pvalues.tsv**: P-values computed using the GSC method. 
- **gso_pvalues.tsv**: P-values computed using the GSO method. 
- **text_pvalues.tsv**: P-values computed through text-mining of PubMed using mapped MeSH terms.


References
----------

Cornish AJ, Filippis I, David A and Sternberg MJE (2015) Exploring the cellular basis of human disease through a large-scale mapping of deleterious genes to cell types. (Under Revision)

[1]: http://alexjcornish.github.io/DiseaseCellTypes/
