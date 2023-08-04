# ECMpy2.0
Automated construction of enzyme-constrained models using ECMpy workflow.

## Create environment

```shell
$ conda create -n ECMpy2 python=3.7  
$ conda activate ECMpy2
```

## Installation
### Installation of ECMpy2.0 using pip
```shell
$ pip install ECMpy2.0
```

### Installation of ECMpy2.0 using github

#### Download ECMpy2.0 is via git clone:
```shell
$ git clone  https://github.com/tibbdc/ECMpy2.0.git
```
#### Install package 
```shell
$ pip install cobra==0.21.0  
$ pip install openpyxl  
$ pip install requests  
$ pip install pebble  
$ pip install xlsxwriter  
$ pip install Bio   
$ pip install Require  
$ pip install quest   
$ pip install scikit-learn  
$ pip install RDKit  
$ pip install seaborn 
$ pip install pubchempy
$ pip install torch
$ pip install ipykernel 
$ pip install bioservices==1.10.4
$ pip install pyprobar
$ pip install xmltodict
$ pip install plotly
$ pip install -U kaleido
$ pip install nbformat
$ python -m ipykernel install --user --name ECMpy2 --display-name "ECMpy2"  
```

## Preprocessing data sources 

The "all--radius2--ngram3--dim20--layer_gnn3--window11--layer_cnn3--layer_output3--lr1e-3--lr_decay0.5--decay_interval10--weight_decay1e-6--iteration50","atom_dict.pickle", "bond_dict.pickle", "edge_dict.pickle", 'fingerprint_dict.pickle", and "sequence_dict.pickle" files are derived from the DLKcat method, and you can update it from GitHub(https://github.com/SysBioChalmers/DLKcat.git).  
The 'bigg_models_metabolites.txt" file is downloaded from BiGG (http://bigg.ucsd.edu/static/namespace/bigg_models_metabolites.txt).  
The "brenda_2023_1.txt" file is downloaded from BRENDA (https://www.brenda-enzymes.org/brenda_download/file_download.php), and "EC_kcat_max.json" is obtained from this file extraction.  
The "gene_abundance.csv" file is downloaded and transformed from PaxDB (https://pax-db.org/download).  
The "uniprot_data_accession_key.json" is compiled from the UniProt database (only for Swiss-Prot), and we have uploaded to zenodo (https://zenodo.org/record/8119567/files/uniprot_data_accession_key.json?download=1).  
The "AutoPACMEN_function.py" file is downloaded and modified from the AutoPACMEN method (https://github.com/klamt-lab/autopacmen.git).  

## Documentation
Full documentation is available at http://ecmpy.readthedocs.io.

## Acknowledgement
Here we are deeply grateful to klamt-lab for releasing the code for AutoPACMEN (https://github.com/klamt-lab/autopacmen) and to SysBioChalmers for sharing the code for DLKcat (https://github.com/SysBioChalmers/DLKcat), which enables ECMpy2.0 to rapidly obtain enzyme kinetics parameter information for the corresponding models. We extend our heartfelt thanks to qLSLab for making the code for GPRuler available (https://github.com/qLSLab/GPRuler), as it has inspired ideas for ECMpy2.0 to automatically acquire the subunit composition of proteins.