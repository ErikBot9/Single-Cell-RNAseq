# Single Cell RNA-Seq
This is a Single Cell RNA-Seq analysis that was carried in collaboration with @ErikBot9. 
The tissue into analysis was a human sample of Substantia Nigra, whose count tables were retrieved from the PanglaoDB repository. The analysis was performed through the Seurat package. 

## LITERATURE ANALYSIS
Before starting with our own workflow, we analyzed the reference results published by Welch et al. and published on the Panglao repository, in which we could see that the identified clusters were oligodendrocytes, neurons, microglia, astrocytes, oligodendrocytes precursors cells and endothelial cells, with PanglaoDB identifying also pancreatic stellate cells. We also checked on PanglaoDB and on the Human Protein Atlas which were the specific markers of these cell types, on which we relied to analyze our results.

## PRE-PROCESSING
Before starting with the analysis, we removed the most problematic cells by plotting the distribution of the number of genes/read, the percentage of mitochondrial DNA and percentage of RNA, then filtering cells according to the outliers of these distributions. 

## ANALYSIS 
We performed a PCA with 10 principal components, obtaining 9 clusters from which we were able to identify and interpret the most significant differentially expressed genes, thanks to whom we were able to detect the cell type related to each cluster.  

## RESULTS
Compared to literature, we found the following cells in accordance:
- Astrocytes
- Oligodendrocytes
- Neurons
- Oligodendrocytes progenitors
- Microglia
- Pancreatic stellate cells

However, Endothelial cells were not identified according to our analysis. 

As newly found cells, we were able to capture:
- Interfascicular, satellite and pre-myelinating oligodendrocytes (three different subtypes of oligodendrocytes)
- Active and ramified microglia
