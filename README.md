
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

The main analysis is provided as an R Markdown workflow. A rendered HTML report is also included so that users can view the full analysis, code chunks, package requirements, generated figures, and outputs directly without re-running the analysis.

## Main analysis report

The complete rendered analysis report can be viewed here:

[Open the HTML report](./reports/SingleCellMultiOmics_Xenopus_analysis.html)


## Repository structure

```text
SingleCellMultiOmics_Xenopus/
│
├── README.md
│
├── rmarkdown reports/
│   └── SingleCellMultiOmics_Xenopus_analysis.html
│
├── data/
│   ├── input_file_1.csv
│   ├── input_file_2.csv
│   └── README_data.md
│
├── figures/
│   ├── figure_1.pdf
│   ├── figure_2.pdf
│   └── supplementary_figure_1.pdf
│
├── results/
    ├── processed_results_1.csv
    ├── processed_results_2.csv
    └── summary_tables/

```

## Folder description

### `rmarkdown/`

This folder contains the main `.Rmd` file used to perform the analysis and generate the final HTML report.

### `reports/`

This folder contains the compiled HTML report generated from the R Markdown file. The HTML report includes the analysis workflow, code chunks, package-loading instructions, results, and automatically generated figures.

### `data/`

This folder contains the input data files required to run the R Markdown analysis. Large files or restricted-access datasets should not be uploaded directly to GitHub. If any data files are too large or cannot be shared publicly, their source or access instructions should be described in `data/README_data.md`.

### `figures/`

This folder contains figures generated automatically from the analysis code or final figure files used in the manuscript.

### `results/`

This folder contains output tables, processed results, and intermediate files generated during the analysis.


## How to use this repository

Users can either view the rendered analysis directly using the HTML report or reproduce the analysis from the R Markdown file.

To reproduce the analysis:

1. Clone this repository.
2. Open the `.Rmd` file in RStudio.
3. Ensure that all required input files are available in the `data/` folder.
4. Knit the R Markdown file to generate the HTML report.

Alternatively, the report can be rendered from R using:

```r
rmarkdown::render("rmarkdown/SingleCellMultiOmics_Xenopus_analysis.Rmd")
```

## Package requirements

The required R packages and installation/loading instructions are included inside the HTML report and the R Markdown file.

## Data availability

Input files used by the R Markdown workflow are provided in the `data/` folder where possible. Any large or restricted-access files should be described in `data/README_data.md`, together with instructions for obtaining the data.

## Citation

If you use this code or analysis workflow, please cite the associated manuscript.
