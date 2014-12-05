Disease Cell Association Data
===

The disease-cell type association data computed using the **DiseaseCellTypes** R-package and text-mining of PubMed. 

**DiseaseCellTypes** R-package is available from: http://alexjcornish.github.io/DiseaseCellTypes. The raw text-mining publication counts are available upon request from a.cornish12@imperial.ac.uk.

The referenced paper details the three methods used to compute disease-cell type association p-values:
- Gene set compactness (GSC)
- Gene set overexpression (GSO)
- Text-mining of the PubMed database. 


Diseases and Cell Types Tested
===========

100 diseases and 73 cell types are tested for associations in the referenced paper using the GSC, GSO and text-mining methods. The results produced (**gsc_pvalues.tsv**, **gso_pvalues.tsv**, **text_pvalues.tsv**) can be downloaded using the links under the page header. 

The text-mining results for a larger set of 406 diseases and 157 cell types (**text_pvalues_large.tsv**) is also provided. The 406 diseases contain the 100 diseases tested in the smaller sets, plus diseases that were excluded from the original analyses for having too few known associated genes. The 157 cell types contain the 73 cell types from the smaller sets, plus cell types represented in the FANTOM5 ontology of cell types (FF) that were excluded for having too little expression data available, low quality expression data, or because they were ancestors or decendants of other cell types, as described by the FF ontology. 


File Descriptions
===========

- **details_cells.tsv**: Matrix of details of the cell types tested. This contains the name we refer to them as (NAME, obtained from FANTOM5), the mapped Cell Ontology ID (CL.ID) and the mapped MeSH terms (MESH). 
- **details_diseases.tsv**: Matrix of details of the diseases tested. This contains the name we refer to them as (NAME, obtained from DisGeNET), the mapped UMLS IDs (UMLS) and the mapped MeSH terms (MESH). 
- **gsc_pvalues.tsv**: Association matrix containing 100 diseases and 73 cell types. P-values computed using the GSC method. 
- **gso_pvalues.tsv**: Association matrix containing 100 diseases and 73 cell types. P-values computed using the GSO method. 
- **text_pvalues_large.tsv**: Association matrix containing 406 diseases and 157 cell types. P-values computed through text-mining of PubMed using mapped MeSH terms.
- **text_pvalues.tsv**: Association matrix ocontaining 100 diseases and 73 cell types. P-values computed through text-mining of PubMed using mapped MeSH terms.


References
===========

Paper under preparation.
