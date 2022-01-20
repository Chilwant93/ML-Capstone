# ML-Capstone- Handwritten Digit Recognition

This is a full project of Handwritten Digit Recognition the model built Pytorch on MNIST Dataset using Sagemaker as Udacity's ML Nanodegree Capstone Project.

# Project Set Up and Installation
AWS Sagemaker studio suing Python 3 (Datascience) kernel
Download MNIST dataset 
Upload to S3 backet
Pytorch library install

# Dataset
Downloaded MNIST Dataset is provide in Datset folder. Whci his downloaded using urls:
https://ossci-datasets.s3.amazonaws.com/mnist/train-images-idx3-ubyte.gz ,
https://ossci-datasets.s3.amazonaws.com/mnist/train-labels-idx1-ubyte.gz ,
https://ossci-datasets.s3.amazonaws.com/mnist/t10k-images-idx3-ubyte.gz ,
https://ossci-datasets.s3.amazonaws.com/mnist/t10k-labels-idx1-ubyte.gz

# Scipt file
The **mnist.py** for hyperparameter training operations, where we train the model numerous times with various hyperparameters and look for the optimum combination based on loss metrics.

# Deployemnt
The endpoint is depolyed 
![alt text](https://github.com/LittleAlchemy/ML-Image_classification_dog_breed/raw/main/screenshots/training%20jobs.png?raw=true)
![alt text](https://github.com/LittleAlchemy/ML-Image_classification_dog_breed/raw/main/screenshots/hyperparameter%20tuning.png?raw=true)

# Result
The summary of training model is provided in profiler report. 

Thank you!
