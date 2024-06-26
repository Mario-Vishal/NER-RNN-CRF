# Named Entity Recognition (NER) using BILSTM and CRF

## Overview
This project implements Named Entity Recognition (NER) using a BILSTM combined with Conditional Random Fields (CRF) in PyTorch. The model is designed to recognize entities in Job Descriptions such as Job Roles, Company Name and Skills.
The Dataset contains 30k Job descriptions which are generated using 12 different job description templates with placeholders to randomly place keywords from a keywords file containing 700 unique keywords which you would find in job descriptions requiring people
from Computer Science department.

## Features
Sequence modeling with BILSTM.<br/>
Sequence labeling with CRF, the file used for crf is directly used from this [repo](https://github.com/rikeda71/TorchCRF/blob/master/TorchCRF/__init__.py]).<br/>
Custom Dataset class which can be used to create DataLoaders for training and testing.<br/>
Custom Class which can generate data suitable for NER in csv format. <br/>

## Requirements
Python - 3.7+
PyTorch - 2.2

## Results
Model Trained for 10 epochs
Achieved an average accuracy of 99.78% on validation data.
