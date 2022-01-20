# ML-Capstone- Handwritten Digit Recognition

This is a full project of Handwritten Digit Recognition the model built Pytorch on MNIST Dataset using Sagemaker to perform Convolutional Neural Network using Pytorch as Udacity's ML Nanodegree Capstone Project.

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
# Training 
The trianing used the pytorch estimator with **mnist.py** script to perform the training job using Convolutional Neural Network. 
![alt text](https://github.com/LittleAlchemy/ML-Capstone/raw/main/Handwritten%20digit%20recognition%20snapshots/training%20jobs.png?raw=true)
# Deployemnt
The endpoint is depolyed 

![alt text](https://github.com/LittleAlchemy/ML-Capstone/raw/main/Handwritten%20digit%20recognition%20snapshots/endpoint.png?raw=true)

The matrics of the depolyed endpiont determoind the CPU usages and memory utilizations during the trining process.
![alt text](https://github.com/LittleAlchemy/ML-Capstone/raw/main/Handwritten%20digit%20recognition%20snapshots/endpoint%20monitor.png?raw=true)
# Result
The results are good with higeh taccuracy for handwritten digit recognition using Pytorch. 
![alt text](https://github.com/LittleAlchemy/ML-Capstone/raw/main/Handwritten%20digit%20recognition%20snapshots/20-%20accuracy%2097.png?raw=true)

| TrialComponentName                           | epochs | hidden_channels | test:accuracy - Min | test:accuracy - Max | test:accuracy - Avg |
|----------------------------------------------|--------|-----------------|---------------------|---------------------|---------------------|
| cnn-training-job-1642600183-aws-training-job | 2.0    | 2               | 95.0                | 97.0                | 96.0                |
| cnn-training-job-1642600790-aws-training-job | 2.0    | 5               | 95.0                | 97.0                | 96.0                |
| cnn-training-job-1642601115-aws-training-job | 2.0    | 10              | 96.0                | 97.0                | 96.5                |
| cnn-training-job-1642601433-aws-training-job | 2.0    | 20              | 95.0                | 97.0                | .0                  |
| cnn-training-job-1642600470-aws-training-job | 2.0    | 32              | 94.0                | 96.0                | 95.0                |
The summary of training model is provided in profiler report. 

Thank you!
