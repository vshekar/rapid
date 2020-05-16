# Rapid
This repo contains code, data and jupyter notebook related to RAPID.

Click this button to access the jupyter notebook without downloading/installing [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/darkreactions/rapid/master?filepath=RAPID.ipynb)

## Repository contents
The following sections indicate the folders which contain code and related data

### Jupyter notebooks

1. RAPID.ipynb - Notebook containing all visualizations
2. Visualization and Statistical Analysis.ipynb - Initial analysis notebook
3. Perovskite learning curve.ipynb - ML code and visualizations notebook

### Raw data
All raw data files are located in the ```data``` folder

1. cifs - Contains the Crystallographic Information Files
2. images - Contains side vial images of each experiment performed
3. xrd/xy - Contains xy files for XRD data
4. 0042.perovskitedata_RAPID.csv - Escalate generated data file including 75 experimental and chemical features. This CSV file is used in visualization and machine learning. (see "Perovskite Dataset Description" for feature explanations)
5. 0042.perovskitedata_RAPID_full.csv - Complete escalate generated data file with all 787 features, including "_raw_" features describing experiment details. The csv file is not used for visualization or machine learning. 
6. image_list.json - Keeps track of all image files in the image folder
7. ml_data.pkl - Python pickle file containing ML results
8. inventory.csv - Chemical inventory data
9. organic_inchikey.csv - Inchi keys and chemical names
10. s_spaces.json - Co-ordinates of state space for each amine

### Scripts
The following python scripts are used in the RAPID.ipynb notebook to generate visualizations

1. plots.py - Generates the reaction outcomes 3D plot widget
2. xrd_plot.py - Generates the xrd plot widget
3. ml_section.py - Generates machine learning outcomes widget
4. cif_plots.py - Generates the cif plot widget. Note that jsmol is used to create the widget