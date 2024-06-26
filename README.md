# Soundfield speech ABR
Code for analysis of subcortical EEG responses to continuous speech presented using insert earphones and in the sound-field. Please cite the following publication if you use this code:
Bachmann, F. L., Kulasingham, J. P., Eskelund, K., Enqvist, M., Alickovic, E., & Innes-Brown, H. (2024). Extending Subcortical EEG Responses to Continuous Speech to the Sound-Field. Trends in Hearing, 28. https://doi.org/10.1177/23312165241246596

# How to use the code
Complete the following steps in order

## Setup filepaths
Modify pathnames.py to point to relevant data and output folders

## Preprocess data
Run preprocess_data.ipynb to load raw EEG data, extract Cz and rereference to linked mastoids, and extract recorded stimulus on Erg1 channel.

## Generate the AN model predictor
Run generate_zilany.ipynb
Rquires python cochlea package https://pypi.org/project/cochlea

## Run analysis of click ERPs and speech TRF
Run main.ipynb in order.

## Generate plots and run statistical tests
Run post_analysis.ipynb in order. 
