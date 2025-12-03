ENGG 680 GROUP 4

To download preprocessed and testing data, use the link below. You still need to download the joint coordinates data from IntelliRehabDS.

https://drive.google.com/file/d/17_PQkPYavjGZpJ5auGj3EFrTNZlFTDfU/view?usp=sharing

X.npy is "ready to train" dataset if you would like to skip data preprocessing step. It can be directly feed into train_model.py

y.npy is also "ready to train" labels respect to X.npy dataset

rehab_cnn_lstm_model_v3.h5 is the latest trained model. It can be directly feed into evaluate.py.

test_heatmaps_npy is "ready to test" unseen dataset so that we can evaluate model reliability better

dataset_skeleton is the simplified joints coordinates data from the intelliRehabDS dataset and we took out 101_18_2_6_1_stand, 105_18_2_7_1_chair, 203_18_2_32_1_wheelchair, 215_18_2_7_1_stand from CORRECT 216_18_2_5_2_stand, 209_18_2_4_2_wheelchair, 211_18_2_2_2_stand, 206_18_2_15_2_chair from INCORRECT for later testing purposes so that they are the unseen testing dataset, which will not be used in model training

ADDED A FEW results visualization files for our presentation

To replicate 

pre. Run DSpreprocesInto2Class and make sure "Simplified" folder is downloaded (We did this step in google collab")

a. Run jointDSpreprocess.py to generate dataset_heatmaps

b. Run make_clips.py to generate trainable X.npy and its relative label y.npy

c. Run train_model.py

d. Run evaluate.py

e. Run test.py

f. Run predict_video.py change file name into one of the eight files we took out earlier
