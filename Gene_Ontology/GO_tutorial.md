![Weill Cornell Medicine Samuel J. Wood Library](../images/WCM_SamWoodLib.png)


# Gene Ontology (GO)
## Understanding gene functions and relationships


```
Peter Oxley, PhD
Associate Director of Research Services

Weill Cornell Medicine
Information Technologies and Services
Samuel J. Wood Library & C.V. Starr Biomedical Information Center
1300 York Avenue Room D-120
New York, NY 10065-4896
(P) 646-962-2576
(F) 212-746-8364
 
pro2004@med.cornell.edu
```

![Library Bioinformatic Service](../images/LBS.png)

__The following are tutorials to accompany the demonstration given for the Library Bioinformatics Service on Monday, May 1st, 2017__

## Browsing the Gene Ontology
1. Navigate in a browser to http://amigo.geneontology.org/amigo
2. Click "Go>>" in the "Browse the ontology" box, or click "browse" in the top menu.
3. Select relevant filters - including organism, and annotation type. This will update the number of terms available in the tree in the viewing pane.
4. To expand a term in the tree, select the "+" icon on the left
5. To view a definition of the term and view the annotations linked to it, click on the term name.
6. To view all annotated products, click "retrieve gene products annotated to this term for this filter set" 

## Searching the Gene Ontology
This section will show you how to use the website feature AMiGO in order to search and browse the ontology for specific terms and annotations. 

1. Navigate in a browser to http://amigo.geneontology.org/amigo

## Analyzing gene enrichment
This section will demonstrate how to identify GO terms that are significantly enriched in a list of genes (eg., differentially expressed genes from an RNA-Seq experiment.)

### Basic enrichment test:
1. Navigate in a browser to http://amigo.geneontology.org/amigo
2. In the Term Enrichment Service box, enter your list of genes
    Accepted IDs for entry (from Panther website):
    * Ensembl: Ensembl gene identifier. Example: "ENSG00000126243"
    * Ensembl_PRO: Ensembl protein identifier. Example: "ENSP00000337383"
    * Ensembl_TRS: Ensembl transcript identifier. "Example: ENST00000391828"
    * Gene ID: EntrezGene IDs. examples include, "GeneID:10203", "10203" (for Entrez gene GeneID:10203)
    * Gene symbol: for example, "CALCA"
    * GI: NCBI GI numbers. Example: "16033597"
    * HGNC: HUGO Gene Nomenclature ids. Example: "HGNC:16673"
    * IPI: International Protein Index ids. Example: "IPI00740702"
    * UniGene: NCBI UniGene ids. Examples: "Hs.654587", "At.36040"
    * UniProtKB:UniProt accession. Example: "O80536"
    * UniProtKB-ID: UniProt ID. Example: "AGAP3_HUMAN"

3. Select the organism represented
4. Click submit

### Advanced enrichment test:
Rather than testing your gene set against all genes annotated for the target organism, it may be more appropriate to choose only those genes that are expressed in the target tissue / environment / condition

1. Navigate to the panther gene enrichment input page:

a. Navigate in a browser to http://amigo.geneontology.org/amigo
b. Select "Advanced" in the Term Enrichment Service box

OR

a. Navigate in a browser to http://pantherdb.org

2. Using the accepted gene IDs, paste your list into the text box, or select a file for upload
3. Select list type "ID list"
4. Select organism
5. Select "Statistical overrepresentation test"
6. De-select "Use default settings"
7. Click "submit"
8. A new window will appear. If you wish to change the reference list that the target gene list will be analyzed against, click "change" button in the "Reference List" box. This will bring up another page, in which you can upload a list of gene IDs (same accepted types as above), to use as the reference set. This page will also let you select the default list for a number of supported organisms (the default list is all genes annotated for that organism).
9. Select the dataset of terms with which you wish to run your analysis. You can choose from the three GO categories (Molecular function, Cellular location, or Biological process), or from one of two pathway datasets (Reactome and PANTHER), or from four PANTHER-curated ontologies.
10. Select whether or not you wish to use a Bonferroni correction for the enrichment analysis.

