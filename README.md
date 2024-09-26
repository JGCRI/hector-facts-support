# hector-facts-extras

[![Active](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/badges/latest/active.svg)

Materials in support of the [Hector-FACTS](https://github.com/JGCRI/hector-facts) workflow and processing results. 


## Description of Contents 

### Data 

|Name                 |Description                                              |
|:--------------------|--------------------------------------------------------:|
| hector-input        |Hector SSP ini and input tables extended to 2500 the end run date for the FACTS|
| hector_params.tgz   |Compressed table of Hector parameters generated by the L0.prep_hector_inputs.R script, this file is also minted on [zenodo](https://zenodo.org/doi/10.5281/zenodo.13774541)| 

### Scripts

| Run Order      |Name                       | Description                                              |
|:---------------|--------------------------:|---------------------------------------------------------:|
|1               | L0.prep_hector_inputs.R   |Uses [Matilda](https://github.com/JGCRI/matilda) to generate the ensmble of Hector parameters that will be used as inputs into Hector-FACTS. This script also compresses the hector_params file and the hector-input directory into the appropriate files for the Hector-FACTS framework|
| 2              |data/get-results.sh     |Launch the Hector-FACTS runs or download the minted results stored on zenodo| 
|3               |Analysis Scripts           |Any of the Rmarkdown files R script here can be run after the Hector-FACTS results are available to process results and generate figures|