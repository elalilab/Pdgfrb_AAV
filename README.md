# Investigating reticuloparenchymal PDGFR-β+ cells in the mouse brain

This repository belong to the Laboratory of Neurovascular Interactions [https://elalilab.com/] at Université Laval, Quebec, Canada 

This repository serves the research project for the investigation of PDGFR-β+ cells after AAV injection.

## Files description

### Folders:

**Models:** This folder contains the brms-fitted models executed in the notebooks. 

**ProData:** Contains processed `.cvs` matrix or data frames generated after data cleaning and pre-processing.

**RawData:** Contains raw `.cvs` or `.tsv` files resulting from CellProfiller or QuPath pipelines. These files are loaded, cleaned and transformed in the different notebooks available in this repository. The final data for analysis and visualization are saved in the **ProData** folder. 

### Individual notebooks:

**Pdgfrb-AAV-Pdgfrb_Morphology.qmd:** This Quarto notebook contains the analysis of morphological features extracted from CellProfiller. It uses as input the data stored in `RawData/Pdgfrb_Morphology`. The cleaned data set used for analysis and visualization is stored in `ProData/Pdgfrb_Morphology.csv`.   

**Pdgfrb-AAV-Pdgfrb_Quantification.qmd:** This Quarto notebook contains the analysis for the cell number in different brain slices and brain regions. The cell counts were generated in QuPath. It uses as input the data stored in `RawData/Pdgfrb_Qunatification`. The cleaned data set used for analysis and visualization is stored in `ProData/Pdgfrb_Annotations.csv`. A visualization for the cell numbers is generated in `Pdgfrb_CellNumber_Vis.ipynb`.

**Pdgfrb_CellNumber_Vis.ipynb:** This Jupyter notebook executes a heatmap visualization for the number of PDGFR-β+ cells estimated in `Pdgfrb-AAV-Pdgfrb_Quantification.qmd`. Please note that the uncertainty is not present. 