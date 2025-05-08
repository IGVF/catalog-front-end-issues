---
name: Feedbacks to UI/Table view
about: Request changes to the table view or change other UI elements for the IGVF
  catalog at https://catalog.igvf.org/
title: "[UI]"
labels: UI
assignees: lidaof, shaneliu0

---

# Template for providing comments + documentation on tables from catalog.igvf.edu
Please provide detailed suggestions for the provided table, for example by completing each of the following sections that you would like changed

### Name of page? (required)
e.g. Variant / Gene / Protein / Region / etc.

### Name of table? (required)
e.g. Enhancer-Gene Model Predictions
Example:
<img width="1178" alt="Image" src="https://github.com/user-attachments/assets/be3b173a-bffc-4828-8a1c-a8f949efdf55" />

### Table title:
Example: X# Enhancer-Gene Model Prediction(s)
### Table title - mouseover help text:
Example: 
This table reports whether the query variant overlaps predicted enhancers, and which genes and cell types are predicted to be linked to that enhancer. Each row reports one predicted target gene and cell type. Distance represents the distance from the query variant to the target gene transcription start site (TSS).
Score: Ranges from 0 (no prediction) to 1 (confident prediction)
Models and datasets: Currently, this table includes predictions from the ENCODE-rE2G model across 1700 ENCODE biosamples (see [Gschwind et al. bioRxiv 2023](https://www.biorxiv.org/content/10.1101/2023.11.09.563812v1.full))
See Documentation (link to documentation)
### Table subtitle:
Example: Which genes are predicted to be regulated by enhancers overlapping this variant?

### Table columns and design:
Options:
• Add a screenshot or link to a mockup (e.g., https://docs.google.com/document/d/1I_b8g9msoaqwko5oJovGsDxd-iyzAKY7myLUat6ytrg/edit?tab=t.0#bookmark=id.tkiprkqs2n46)
• Write the design of the table using markdown table syntax
• Edit the text template below: 
Columns:  (Column Name (hyperlink if applicable) [API query details, if known]
• Cell Type 
• Target Gene
• Score
• Dataset 
• Model
• Distance to gene TSS
### Sortable columns for table:
Example: Cell Type, Target Gene, Score, Model, Distance to gene TSS
### Filterable columns for table:
Example: Cell Type, Target Gene, Model
### API details or filtering:
Example: Only show cases where Model == ENCODE-rE2G-DNaseOnly
### Documentation (or, send a PR at the [docs repo](https://github.com/twlab/igvf-catalog-docs)): 
Link: https://docs.catalog.igvf.org/nodes/variant#enhancer-gene-model-prediction-table
Example:
This table shows which genes are predicted to be regulated by enhancers overlapping the query variant. Each row reports one predicted target gene and cell type. 
Column | Description
-- | --
Cell Type | The specific cell type for the prediction
Target Gene | The gene predicted to be regulated (click to view more details)
Score | The strength of the prediction (range: 0 to 1, higher indicates a more confident prediction)
Dataset | The source dataset (click for more information)
Model | The predictive model used
Variant-Gene Distance | Genomic distance between the variant and gene body

Currently, this table includes predictions from the ENCODE-rE2G model across 1700 ENCODE biosamples (see [Gschwind et al. bioRxiv 2023](https://www.biorxiv.org/content/10.1101/2023.11.09.563812v1.full))
The table is initially sorted by Score in descending order, showing the strongest predictions first.

### Any additional UI elements or other details?
