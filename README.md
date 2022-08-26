# ECNN-C
* Code for paper: ECNN-C:EEG-based Emotion Recognition via Efficient Convolutional Neural Network and Contrastive Learning
# About the paper  
* Title: ECNN-C:EEG-based Emotion Recognition via Efficient Convolutional Neural Network and Contrastive Learning  
* Authors: Chang Li, Xuejuan Lin, Yu Liu, Rencheng Song, Juan Cheng, and Xun Chen  
* Institution: HeFei University of Technology   
* Published in: IEEE Sensors Journal  
# Instructions
* Before running the code, please download the DEAP and DREAMER datasets, unzip it and place it into the right diectory. The DEAP dataset can be found here. The DREAMER dataset can be found here. Each.mat data file contains the EEG signals and consponding labels of a subject. 
* First, you need to preprocess the two data sets. The EEG data should be segmented using a sliding window of 128 points over 1s for each subject. On the DEAP dataset, each subject have 40 experimental signals, and each subject could be divided into 60 segments, so each subject has 2400 EEG samples with a size of 32 x 128. On the DREAMER dataset, 3278 EEG samples are obtained on average for each subject with a size of 14 x 128.
* Then, after preprocessing, the original .mat data files are converted to .pkl data files. (For detailed preprocessing code, refer to the deap_pre_process.py in the gcForest.)
* You should modify the 'dataset_dir' in the data.py file based on the location of your datasets.
* Using main.py to train and test the model (10-fold cross-validation).
# Requirments
* python>=3.7
* pytorch>=1.4.0
* torchvision>=0.8.1
* Numpy>=1.19.2
* librosa>=0.8.0  
If you have any questions, please contact xuejuanlin@mail.hfut.edu.cn
# Reference
* gcForest

