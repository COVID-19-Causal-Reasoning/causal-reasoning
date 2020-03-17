## Data Standards

### a. Shared data set should be in .csv format with headers

### b. Headers have to be standardized using the following data standards

Node standard reference table

|  ﻿CODE  | NODE_TYPE  | COLUMN_NAME  | DESCRIPTION  | 
| ---- | --- | --- | --- | 
|  D  | DRUGS  | DRUG_NAME  | Drug name  | 
|  D  | DRUGS  | DRUG_SMILES  | SMILES of the drug  | 
|  D  | DRUGS  | DRUG_DBID  | Drugbank ID (https://www.drugbank.ca/)  | 
|  D  | DRUGS  | DRUG_CASID  | CAS Registed Number  | 
|  D  | DRUGS  | DRUG_CID  | Pubchem ID (https://pubchem.ncbi.nlm.nih.gov/)  | 
|  P  | VIRAL_SPECIES  | VIRAL_SPECIES_NAME  | Species name of the virus  | 
|  P  | VIRAL_SPECIES  | VIRAL_TAXID  | Tax id of the virus (https://www.ncbi.nlm.nih.gov/taxonomy)  | 
|  P  | VIRAL_SPECIES  | VIRAL_FAMILY_NAME  | Species name of the virus family  | 
|  P  | VIRAL_SPECIES  | VIRAL_FAMILY_TAXID  | Tax id of the virus family (https://www.ncbi.nlm.nih.gov/taxonomy)  | 
|  V  | VIRAL_TARGET  | VIRAL_TARGET_NAME  | Virus target name with species information  | 
|  V  | VIRAL_TARGET  | VIRAL_UNIPROTID  | Uniprot ID for virus target (https://www.uniprot.org/)  | 
|  V  | VIRAL_TARGET  | VIRAL_GENE_ID  | Gene ID for virus target (https://www.ncbi.nlm.nih.gov/gene/)  | 
|  V  | VIRAL_TARGET  | VIRAL_GENE_SYMBOL  | Gene symbol for virus target  | 
|  V  | VIRAL_TARGET  | VIRAL_TARGET_SPECIES  | Species name for virus target  | 
|  V  | VIRAL_TARGET  | VIRAL_TARGET_TAXID  | Species tax id for virus target (https://www.ncbi.nlm.nih.gov/taxonomy)  | 
|  H  | HOST_TARGET  | HOST_TARGET_NAME  | Human target name  | 
|  H  | HOST_TARGET  | HOST_UNIPROTID  | Uniprot ID for human target (https://www.uniprot.org/)  | 
|  H  | HOST_TARGET  | HOST_GENE_ID  | Gene ID for human target (https://www.ncbi.nlm.nih.gov/gene/)  | 
|  H  | HOST_TARGET  | HOST_GENE_SYMBOL  | Gene symbol for human target  | 
|  H  | HOST_TARGET  | HOST_TARGET_SPECIES  | Human  | 
|  H  | HOST_TARGET  | HOST_TARGET_TAXID  | 9606  | 
|  W  | HOST_PATHWAY  | HOST_PATHWAY_NAME  | Human pathway name  | 
|  W  | HOST_PATHWAY  | HOST_PATHWAY_KEGGID  | Human pathway KEGG ID (https://www.kegg.jp/)  | 

Link standard reference table

|  ﻿LINK_TYPE  | NODE_1  | NODE_2  | EVIDENCE  | EVIDENCE_TYPE  | LINK_VALUE  | CONFIDENCE_SCORE  | CITATION  | DESCRIPTION  | 
| ---- | --- | --- | --- | --- | --- | --- | --- | --- | 
|  VHI  | VIRAL_TARGET_NAME  | HOST_TARGET_NAME  | ASSAY  |   |   |   |   |   | 
|  HHI  | HOST_TARGET_NAME  | HOST_TARGET_NAME  | ASSAY  |   |   |   |   |   | 
|  HWI  | HOST_TARGET_NAME  | HOST_PATHWAY  | INFORMATICS  | ENRICHMENT  |   |   |   |   | 
|  DVI  | DRUG_NAME  | VIRAL_TARGET_NAME  | ASSAY  | BIOCHEMICAL  | IC50 (M),Ki(M),Kd(M)  | PX  |   |   | 
|  DVI  | DRUG_NAME  | VIRAL_GENE_SYMBOL  | ASSAY  | EXPRESSION  | Fold change  | FC  |   |   | 
|  DHI  | DRUG_NAME  | HOST_TARGET_NAME  | ASSAY  | BIOCHEMICAL  | IC50 (M),Ki(M),Kd(M)  | PX  |   |   | 
|  DHI  | DRUG_NAME  | HOST_GENE_SYMBOL  | ASSAY  | EXPRESSION  | Fold change  | FC  |   |   | 
|  DPI  | DRUG_NAME  | VIRAL_SPECIES_NAME  | ASSAY  | PHENOTYPIC  | EC50 (M)  | PX  |   |   | 
|  DDS  | DRUG_NAME  | DRUG_NAME  | SIMILARITY  | COMPARE  | 0-1  |   |   |   | 
|  VVS  | VIRAL_SPECIES_TARGET_NAME  | VIRAL_SPECIES_TARGET_NAME  | SIMILARITY  | COMPARE  | 0-1  |   |   |   | 
|  HHS  | HOST_TARGET_NAME  | HOST_TARGET_NAME  | SIMILARITY  | COMPARE  | 0-1  |   |   |   | 
|  PPS  | VIRAL_SPECIES_TARGET_NAME  | VIRAL_SPECIES_TARGET_NAME  | SIMILARITY  | COMPARE  | 0-1  |   |   |   | 

[Example data](https://ghddiai.oss-cn-zhangjiakou.aliyuncs.com/file/data_example.csv)
