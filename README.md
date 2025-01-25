# Metagenome_functional_clustering
Data processing and analysis code for the manuscript titled, ["Metagenomic clustering links specific metabolic functions to globally relevant ecosystems"](https://journals.asm.org/doi/10.1128/msystems.00573-24) by Zach Flinkstrom, Sam Bryson, Pieter Candry and Mari Winkler.
## About this repository
* Dataset files can be retrieved from this [figshare project](https://figshare.com/projects/Metagenome_functional_clustering/187989) and be placed in the `data/` directory. The dataset files are stored in [anndata](https://anndata.readthedocs.io/en/latest/) objects which are saved in the HDF5 file format. This allows for the gene abundance matrix to be linked to metadata about the genes and about the metagenome samples all in one file.
* The `Data_preprocessing.ipynb` notebook contains code to filter and normalize the raw dataset. This includes operations like removing samples below a certain sequencing depth and ensuring all samples went through the JGI annotation pipeline. In addition it performs the data matrix normalization that is based off of the [ALDEx2](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4030730/) methodology.
* The `Data_analysis.ipynb` notebook contains all of the analysis and plotting code from the project. This includes basic dataset description, sample clustering, and marker gene analyses.
* The `Taxonomy_analysis.ipynb` notebook looks at the taxonomic composition of the dataset metagenomes, pulling from the zip files in the data folder.
## Dependencies
This repository was created and run using python (3.6.10) and makes use of the following packages with version in parentheses:
* numpy (1.19.5)
* pandas (1.1.5)
* geopandas (0.6.1)
* anndata (0.7.6)
* scanpy (1.7.2)
* scipy (1.5.4)
* scikit-posthocs (0.7.0)
* scikit-bio (0.5.6)
* scikit-learn (0.24.2)
* matplotlib (3.3.4)
* seaborn (0.11.1)
* plotly (5.3.1)
* collections (python standard library)
* random (python standard library)
* json (python standard library)
* os (python standard library)
* glob (python standard library)
