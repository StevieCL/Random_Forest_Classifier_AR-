# Random_Forest_Classifier_AR-

This is a project that I developed, together with my colleague Natalia Fuentes Medina, to present it as a final project in the subject 'Biomolecule Engineering'. 
This Machine learning model was made to classify whether a compound exhibits biological  activity (agonist)  or not at the human nuclear androgen receptor (AR). 
The data used is available in PubChem; these are results of qHTS bioassays  conducted in the U.S. Tox 21 program. The model presented here is the first iteration 
of what would be a more complex model in the future. At the beginning of the project, you can see that the analysis is done based on a property of the compounds 
which is  'Ratio Potency', this is because initially the model was thought as a regression model that predicted said property for each  compound, since the objective
was to make a model that would be used to design chemical molecules that have high affinity for  the human nuclear androgen receptor to synthesize anabolic steroids 
closely related to its receptor. It is important to emphasize  that what is presented is a first iteration of the final model.

## Notebooks description: 

* **n_Data_exploration:** This notebook explores the data downloaded from PubChem (AID_743053_datatable_all.csv), performs data cleansing and other necessary fixes from 
the chemical analysis that is carried out as the project develops.

* **n_Exploratory_data_analysis:** This notebook performs a brief chemical-statistical analysis of the data that resulted from n_Data_exploration.

* **n_Data_Model:** In this notebook the data is prepared to be able to train the model; PubChem fingerprints for each compound are calculated using PaDEL software.

* **n_ML_model:** The model (Random forest classifier) is created, trained and evaluated. Many conclusions are made from what is obtained.

## Bibliography:

* Chemical Genomics Profiling of Environmental Chemical Modulation of Human Nuclear 
  Receptors. Author(s): Ruili Huang, Menghang Xia, Ming-Hsuang Cho, Srilatha Sakamuru, Paul Shinn,
  Keith A. Houck, David J. Dix, Richard S. Judson, Kristine L. Witt, Robert J. Kaylock,
  Raymond R. Tice and Christopher P. Austin. Source: Environmental Health Perspectives, Vol. 119, No. 8 (AUGUST 2011), pp. 1142-1148.
  Published by: Brogan & Partners. Stable URL: http://www.jstor.org/stable/41233470 .
  
  
## Databases: 
* qHTS results data: https://pubchem.ncbi.nlm.nih.gov/bioassay/743053 
* qHTS used compounds with their chemical properties information: https://www.ncbi.nlm.nih.gov/pcsubstance?term=%22Tox21%22%5BSourceName%5D%20AND%20hasnohold%5Bfilt%5D
