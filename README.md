# CODEX-CML-BM


## Introduction

This project’s data analysis is based on the Enable Medicine platform (https://www.enablemedicine.com), which provides an end-to-end workflow for data processing and interpretation. Some of the code packages used in our analysis were internally developed by Enable Medicine and are designed to function exclusively within this platform, so we are unable to share them.

However, we are publicly sharing our analysis pipeline to provide insights into our approach and to help others develop their own workflows. We hope this resource serves as a useful reference for researchers working on similar projects.


## Analysis Workflow

- **Segmentation** – This step is performed directly through the Enable Medicine portal.  

- **Clustering and subclustering** – Unsupervised clustering of all cells to identify major populations.  

- **Supervised cell type annotation** – This step is performed directly through the Enable Medicine portal.  

- **Fat cell and megakaryocyte incorporation** – These two cell types had weak or unusually shaped nuclear signals, which were poorly captured by our segmentation approach. To remedy this, a manual approach was used to mark the locations of these cell types in the dataset. Subsequently, the centroids of each manually identified cell were calculated and incorporated into the dataset.  

- **Neighborhood analysis** – Identification and characterization of spatially associated cell populations to understand local cellular microenvironments.  

- **Neighborhood differential enrichment** – A significant coefficient in this model indicates a differential abundance of a specific cell type within a given neighborhood, highlighting its enhanced enrichment in one group compared to the other.  

- **Pairwise adjacency analysis** – Pairwise contact analysis identified preferentially co-located pairs of cell types.  

This shared pipeline provides a structured approach to spatial and single-cell data analysis, allowing researchers to adapt and refine it based on their specific needs.
