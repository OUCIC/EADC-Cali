# Enhanced High-Speed ADC Calibration: 
We release the code of Enhanced High-Speed ADC Calibration: A JointApproach for Dynamic and Static Errors via Temporal Error Learning in our papers:
## Introduction
We propose an integrated calibration neural network. The network is meticulously structured into two key components:error extraction and error fitting. Within the error extraction component, we employ temporal convolutional network (TCN) to extract the local and long-term features, from the ADC output sequences. The error fitting component, comprising a three-layer FCNN, is designed to finally fit the error in the ADC output.
![image](Fig.1.png)

## Requirements
* Python 3.11.8
* Pytorch 2.2.1
* CUDA 12.1
  ```
  pip install -r requirements.txt
  ```
## Datasets
We will provide the ADC datasets and analysis methods later.
## Usage
The network framework is contained in folder, with the following structure:
```
models.py
utils.py
train.py
test.py
```
To run this network, you need to train the network model by running ```train.py``` then run ```test.py```to obtain the network output results for subsequent analysis.
## Acknowledgement
We really appreciate the contributors of following codebases.

[TCN] (http://github.com/locuslab/TCN)
