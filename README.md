# Metagenome_functional_clustering
Data processing and analysis code for the manuscript titled, "Metagenomic clustering links specific metabolic functions to globally relevant ecosystems" by Zach Flinkstrom, Sam Bryson, Pieter Candry and Mari Winkler.
## About this repository
* Dataset files can be retrieved from this [figshare project](https://figshare.com/projects/Metagenome_functional_clustering/187989) and be placed in the `data/` directory. The dataset files are stored in [anndata](https://anndata.readthedocs.io/en/latest/) objects which are saved in the HDF5 file format. This allows for the gene abundance matrix to be linked to metadata about the genes and about the metagenome samples all in one file.
* The `Data_preprocessing.ipynb` notebook contains code to filter and normalize the raw dataset. This includes operations like removing samples below a certain sequencing depth and ensuring all samples went through the JGI annotation pipeline. In addition it performs the data matrix normalization that is based off of the [ALDEx2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4030730/) methodology.
* The `Data_analysis.ipynb` notebook contains all of the analysis and plotting code from the project. This includes basic dataset description, sample clustering, and marker gene analyses.
* The `Taxonomy_analysis.ipynb` notebook looks at the taxonomic composition of the dataset metagenomes, pulling from the zip files in the data folder.
## Dependencies
This repository requires on the following python packages:
* numpy
* pandas
* geopandas
* anndata
* scanpy
* scipy
* scikit_posthocs
* skbio
* sklearn
* collections
* random
* json
* os
* glob
* matplotlib
* seaborn
* plotly
