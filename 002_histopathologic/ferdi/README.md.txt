This folder has 4 different colab scripts:

- Preprocessing_script_for_local: Download the files in local and then classify the train labels in two different folders to apply flow_from_directory keras function.

- Histopatological_for_local: After the preprocessing, apply a NN from google drive.

- Histopatological_all_colab_(...): Download the data directly from kaggle and process everything in colab (no local). There is a script with a small NN (75% accuracy) and another one with a large NN (92% accuracy). This script uses flow_from_dataframe keras function.
