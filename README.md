# Introduction
The project consists of four components: 1. Scripts (Python scripts and MATLAB scripts) 2. Figures 3. Data 4. Scenarios.
# Scripts Part
The post-processing program for handling PartMC-MOSAIC data is `'NC_X.py'`, written in Python. When importing `NC_X`, please ensure that both `'NC_X.py'` and it are present in the current working directory. The way to use these scripts is listed in `'~/python/README.txt'`.
# Figures Part
The figures used in the manuscript and supplementary information are displayed in the directory path `'~/Figure/'`.

      
 


# Data Part
The data for plotting will be stored in the path `'~/Data/'`. Among these, the file `'Dp_Dc_Conc.csv'` stores information about particle diameter (Dp), core diameter (Dc), and number concentration. Due to its large size, it has not been uploaded to the project. You can compute and store the data by running the script `'~/python/saveDcDpconc.py'`. Here are the specific instructions:
1.	Make sure that the current working directory is   `'~/python/'`.
2.	Run the command `'python saveDcDpconc.py'`.

# Scenarios Part
Scenario 1 and Scenario 2 store the raw data and scenario settings for Figure 1-3 and Figure 4, respectively. Taking `'Scenario 1'` as an example, the raw data is in NC format and can be found in the path `'~/1_scenario/out/'`. The files with the `'.dat'` extension are the input files required for running `PartMC`, while those with the `'.spec'`extension are control panels for managing the corresponding `'.dat'` files for each input section. `PartMC` runs through a Docker image, and the specific command can be found in `'~/1_scenario/run.sh'`. To run the PartMC program, simply run the command `./shell.sh`.
