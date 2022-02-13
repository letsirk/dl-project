# Deep Learning Project (05/2019)

## Introduction

A project for [Kaggle competition about categorizing animals in the wild](https://www.kaggle.com/c/iwildcam-2019-fgvc6) using deep learning based methods. The purpose of this project is to implement a CNN-based model for image classification task. Therefore, the solution utilizes the arhictecture of [YOLOv3](https://pjreddie.com/media/files/papers/YOLOv3.pdf) model by implementing the Darknet-53 backbone and its head from scratch using PyTorch library. The assembled model is trained and validated using the datasets provided in the Kaggle competition. A submission with a low score was achieved. The detailed information about the project and its results can be found [here](https://github.com/letsirk/dl-project/blob/master/deep-learning-project-report.pdf). 

Furthermore, the project was accomplished during *Deep Learning* course with an aim of contributing towards my Master's thesis, [Increasing the safety in the proximity of the mobile working machines: a study of detecting people](http://urn.fi/URN:NBN:fi:aalto-202110249676), that takes advantage of the [Scaled-YOLOv4](https://arxiv.org/abs/2011.08036) model. 

## Techniques and Tools
The project utilizes following techniques and tools:
* Python and Jupyter Notebook 
  * [scikit-learn](https://scikit-learn.org/stable/) library to access general metrics (e.g. confusion matrix and accuracy score)
  * [PyTorch](https://pytorch.org/) library to access Deep Learning functionalities and CUDA resources
  * other general libaries to manipulate and show data (pandas, seaborn, matplotlib, numpy) 

## Instructions

### 1. Download the Dataset
iWildCam 2019 - FGVC6: [https://www.kaggle.com/c/iwildcam-2019-fgvc6](https://www.kaggle.com/c/iwildcam-2019-fgvc6)
* get the dataset files
* extract them to following folders:
  * \input\test.csv
  * \input\train.csv
  * \input\test_images\
  * \input\train_images\
  * \input\iwildcam-2019-fgvc6\sample_submission.csv
 
### 2. Preprocess the Dataset
* run reducing-image-sizes-to-32x32.ipynb
* copy the created files to \input\preprocess\changing-image-dimensions-to-3x32x32\
  
### 3. Run the Code
* Pytorch CNN model with Darknet-53 architecture: [dl-project-code](https://letsirk.github.io/dl-project/)
