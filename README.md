# Visual-Recognition-HW4
NCTU Visual Recognition Homework 4

## Hardware
OS: Ubuntu 18.04.3 LTS

CPU: Intel(R) Xeon(R) W-2133 CPU @ 3.60GHz

GPU: 1x GeForce RTX 2080 TI

## Reproducing Submission
To reproduct my submission without retrainig, do the following steps:
1. [Installation](#installation)
2. [Dataset Preparation](#Dataset-Preparation)
3. [Training detail](#Training)
4. [Testing detail](#Testing)
5. [Reference](#Reference)

## Installation

this code was trained and tested on Ubuntu 18.04

```
cd /path/to/your/zssr/
conda env create -f environment.yml

```

## Dataset Preparation
```
cs-t0828-2020-hw4

├── HW4
│   ├── pytorch-ZSSR 
│   │   ├── kernel_example
│   │   │   ├── Put your image and corresponding kernel here


```
I try a lot of combination between image and kernel, you can try your own combination.

## Training
To train models:

```
cd /path/to/your/zssr/
python run_ZSSR.py X2_GIVEN_KERNEL_CONF
```

The expected training times are:
Model | GPUs | Training Iteration | Training Time
------------ | ------------- | ------------- | -------------
zssr | 1x RTX 2080Ti | 5000 | 5 minutes (each image)


## Testing
To test models:

```
cd /path/to/your/zssr/
python run_ZSSR.py X2_GIVEN_KERNEL_CONF
```

## Reference
1. [zssr](https://github.com/assafshocher/ZSSR).
