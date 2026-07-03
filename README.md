
# Tissue-specific chromatin accessibility and co-factor availability together define Ascl1-dependent neural reprogrammability across germ layers during embryogenesis

**David Lando<sup>1,\*</sup>, Samina Kausar<sup>1,\*</sup>, Toshiaki Shigeoka<sup>1,2</sup>, Frances Connor<sup>1</sup>, Jerome Jullien<sup>3</sup> and Anna Philpott<sup>1,4,†</sup>**

<sup>1</sup> Cambridge Stem Cell Institute, University of Cambridge, Cambridge CB2 0AW, UK  
<sup>2</sup> Division of Biological Science, Nara Institute of Science and Technology (NAIST), Ikoma-shi, Nara, Japan  
<sup>3</sup> Center for Research in Transplantation and Translational Immunology, University of Nantes, Nantes, 44000, France  
<sup>4</sup> Department of Oncology, University of Cambridge, Cambridge CB2 0AH, UK  

<sup>\*</sup> These authors contributed equally to this work  
<sup>†</sup> To whom correspondence should be addressed  

**Keywords:** Ascl1, single-cell multiomics, chromatin accessibility, cell competence, neural reprogramming, Xenopus development

---

# SingleCellMultiOmics_Xenopus
This repository contains the code, analysis files, input data, and figure-generation outputs associated with the manuscript:

**Tissue-specific chromatin accessibility and co-factor availability together define Ascl1-dependent neural reprogrammability across germ layers during embryogenesis**

The main analysis is provided as an R Markdown workflow. 

## Main analysis report

This report contains the R Markdown workflow used to analyse single-cell multiomics and related genomic datasets for the study of Ascl1-dependent neural reprogramming in the developing *Xenopus* embryo. The report includes executable code, package requirements, analysis outputs, and automatically generated figures associated with the manuscript.

The goal of this report is to provide the key analysis steps required to reproduce the main results. Code for these important steps is included directly within the report.

[Open the HTML report](./rmarkdown_report)


## Repository structure

```text
SingleCellMultiOmics_Xenopus/
│
├── README.md
│
├── rmarkdown_report/
│   └── SingleCellMultiOmics_Xenopus_analysis.html
│
├── data/
    ├── Xenopus_scRNA_Data_allSublibraries
    ├── Xenopus_scATAC_Data_allSublibraries
    ├── protein_coding_introns.rds
    ├── gene_lists
    └── HOMER_motif_analysis



```

## Folder description

### `rmarkdown_report/`

This folder contains the compiled HTML report generated from the R Markdown file. The HTML report includes the analysis workflow, code chunks, package-loading/package requirements, results, and automatically generated figures. 

### `data/`

This folder contains the input data files required to run the R Markdown analysis. Only one larger file specifically **data/Xenopus_scATAC_Data_allSublibraries/FragmentFile_filtered_Ascl1_T1_barcodes_cutoff1000.tsv.gz** is not uploaded directly to GitHub but can be doanloaded from Gene Expression Omnibus data repository (GEO) with the accession number **GSE336320** for the multiome snRNA/ATACseq data. 

## How to use this repository

Users can either view the rendered analysis directly using the HTML report or reproduce the analysis from the R Markdown file, which can be provided upon request.

To reproduce the analysis:

1. Download or clone this repository.
2. Open the `.Rmd` file in RStudio.
3. Ensure that all required input files are available in the `data/` folder and that file paths are set up correctly.
4. For the transcriptomic modality, unzip all sublibrary folders in `data/Xenopus_scRNA_Data_allSublibraries`.
5. Genome annotation and reference genome files are not included in the `data/` folder. The required `.gtf` annotation file and `.fa` genome sequence file can be obtained from the *Xenopus laevis* NCBI RefSeq genome assembly **GCF_017654675.1**.
6. Knit the R Markdown file to generate the HTML report.


## Package requirements

The required R packages are included inside the HTML report and the R Markdown file.

## Data availability

Input files used by the R Markdown workflow are provided in the `data/` folder where possible. Sequencing data has been deposited in the GEO repository with the accession number **GSE230767** for the ChIP-seq data and **GSE336320** for the multiome snRNA/ATACseq data.


