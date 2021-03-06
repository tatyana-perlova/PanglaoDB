# PanglaoDB
This repo contains data and metadata from the database https://PanglaoDB.se

# *data* directory
Files contain comma-delimited tables without headers.

## *sample_clusters* directory
Contains cell clustering results.

## cell_type_abbrev.txt
Maps cell types to abbreviations.


| Column | Description
| ------------- |:-------------
| 1 | Cell type
| 2 | Abbreviation

## cell_type_annotations.txt
Mapping cell clusters to cell types.

| Column | Description
| ----------- |:----------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | Cell type annotation
| 5 | P-value from Hypergeometric test
| 6 | Adjusted p-value (BH)
| 7 | Cell type Activity Score

## cell_type_annotations_markers.txt
Markers that were used to determine the cell type.

| Column | Description
| -------- |:---------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | Gene symbol

## cell_type_desc.txt
Cell types and their descriptions.

| Column | Description
| -------- |:--------
| 1 | Cell type
| 2 | Biological description of this cell type
| 3 | Possible synonyms

## clusters_to_number_of_cells.txt
Clusters to number of cells

| Column | Description
| -------- |:--------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | Number of cells

## cyclone.txt
Results from cell cycle analysis based on cyclone.

| Column | Description
| ------- |:----------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | % cells in G1
| 5 | % cells in G2M
| 6 | % cells in S

## expressed_tx_list.txt
Expressed transcription factors.

| Column | Description
| ------ |:----------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | Gene encoding the transcription factor

## genes.txt
Gene symbols used.

| Column | Description
| ------- |:------------
| 1 | Ensembl gene ID
| 2 | Gene symbol

## germ_layers.txt
Cell types to organs and germ layers.

| Columns | Description
| ------- |:--------------
| 1 | Cell type
| 2 | Germ layer
| 3 | Organ

## metadata.txt
Sample metadata.

| Columns | Description
| -------- |:-------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Tissue origin of the sample
| 4 | scRNA-seq protocol
| 5 | Species
| 6 | Sequencing instrument
| 7 | Number of expressed genes
| 8 | Median number of expressed genes per cell
| 9 | Number of cell clusters in this sample
| 10 | Is the sample from a tumor? (1 true otherwise false)
| 11 | Is the sample from primary adult tissue?
| 12 | Is the sample from a cell line?

## mito.txt
Mitochondrial expression.

| Columns | Description
|-------- |:--------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | z-score
| 5 | P-value
| 6 | Adjusted p-value
| 7 | Mean perc mito reads

## regulons.txt
| Columns | Description
| ------ |:----------
| 1 | SRA accession
| 2 | SRS accession
| 3 | Cluster index
| 4 | Transcription factor gene
| 5 | TF binding site motif
| 6 | Confidence (AUC)
| 7 | Genes controlled by this TF

# Contact
* Oscar Franzén <p.oscar.franzen@gmail.com>

# Reference
* Franzén,O., Gan,L.-M. and Björkegren,J.L.M. PanglaoDB: a web server for exploration of mouse and human single-cell RNA sequencing data. Database (2019) Vol. 2019: doi:10.1093/database/baz046
