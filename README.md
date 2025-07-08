# Alzheimers-MRI-Predictor

![image](https://img.shields.io/badge/License-GNU_GPL_v3.0-slateblue.svg)

![image](https://github.com/user-attachments/assets/d7817a0a-6cde-4151-8b1c-2e16bd672a14)

## Overview

This is a Python-based machine learning-trained image scanning notebook and algorithm for predicting the presence and severity of Alzheimer's disease. As of right now it is a purely back-end project and must be run as a notebook or otherwise in a coding environment, but it is viable.

## Development

This is a portfolio project that I created in June and July of 2025 with the idea of eventually creating a publicly accessible medical diagnostic tool.

## Instructions for Use - Streamlined version, for general usage
* Please download the following files to the same directory: STREAMLINED_Alzheimers_MRI_Detector_Final_Version.ipynb, Alzheimers_Test_Dataset.parquet, Alzheimers_Train_Dataset.parquet, and best_dualpool201_model.keras.
* Please download any sample png images if you wish into the same directory.
* Again, for general usage, **_please use the "STREAMLINED" version_**.
* Please install Python 3 (code has been verified in Python 3.11), and please install any dependencies in the Dependencies section below if you do now already have them.
* Please run the STREAMLINED_Alzheimers_MRI_Detector_Final_Version.ipynb notebook in a proper coding environment. It may take up to ~10 minutes but can run on most rigs.
* Adjust parameters in the image predictor code blocks as desired for subsequent runs. There is also a toggle to stop the Run All just before the loading and training blocks if you wish to use it.
* If you have an overhead MRI scan you wish to evaluate, please keep it in the directory and have it named accordingly, as test##.jpg with the '##' part replaced by a number from 01 to 20.
* JPEG images are vastly more accurates since that was the file type from the Parquet dataset.
* Images larger than 128 x 128 will be resized. Images smaller than that will be rejected.

## Optional Instructions for original version - most will be redundant
* Please download the following files to the same directory: Alzheimers_MRI_Detector_Final_Version.ipynb, Alzheimers_Test_Dataset.parquet, Alzheimers_Train_Dataset.parquet, and best_dualpool201_model.keras.
* Please download any sample png images if you wish into the same directory.
* Please run the Alzheimers_MRI_Detector_Final_Version.ipynb notebook in a proper coding environment.
* _**If you wish to skip the training step**_, as the repository already has the trained model included, please skip down to the block titled MANUAL HARD STOP and uncomment the line ```# raise SystemExit("🛑 Manual checkpoint: stopping execution here.") # Comment out when not in use``` so that it stops the program before the training step.
* Please run the Alzheimers_MRI_Detector_Final_Version.ipynb notebook in a proper coding environment. Please be advised that if you are including training, it may take quite some time if you're doing it locally without a powerful rig. It should automatically compile and train itself based on the parameters, or otherwise load the present CNN keras file and also save it. If you skip the training, please utilize the Manual Hard Stop feature as described above and execute the cells after it manually.
* Adjust parameters in the image predictor code blocks as desired. There is also a toggle to stop the Run All just before the loading and training blocks if you wish to use it.
* If you have an overhead MRI scan you wish to evaluate, please keep it in the directory and have it named accordingly, as test##.jpg with the '##' part replaced by a number from 01 to 20.
* JPEG images are vastly more accurates since that was the file type from the Parquet dataset.
* Images larger than 128 x 128 will be resized. Images smaller than that will be rejected.


## Required Dependencies/Imports
* panda
* numpy
* tensorflow
* scikit-learn
* scikit-image
* io
* os
* random
* seaborn
* matplotlib
* PIL
* pyarrow
* opencv-python
#### Optional Imports (only used for code cell timestamps)
* datetime
* zoneinfo

## License
This site is licensed under the [GNU General Public License v3.0](https://choosealicense.com/licenses/gpl-3.0/). Feel free to share and modify it, but please just give accurate attribution to the source and the writer and state any significant changes, and please don't change the license under which it is exported.

### © Dan McKay 2025
