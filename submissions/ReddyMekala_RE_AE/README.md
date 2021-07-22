# Classifying User Requirements from Online Feedback in Small Dataset Environments using Deep Learning 

## Summary of Artifact

This artifact (Artifact location: https://doi.org/10.6084/m9.figshare.14273594) contains the dataset, code and models (both pre-trained and fine-tuned) that we have used in our study. 
The study uses three deep learning models (BERT, ELMo and FastText) and two traditional machine learning models (Naive Bayes and TF-IDF/SVM).

This guide can be used either as a starting point for new research in this
area or as a replication or reproduction of the research reported in our RE 2021 paper.

## Author Information

The authors of this study are Rohan Reddy Mekala, Asif Irfan, Eduard C. Groen, Adam Porter, and Mikael Lindvall.

If you use this study to support your research please provide attribution by
citing the following:

R. R. Mekala, A. Irfan, E. C. Groen, A. Porter and M. Lindvall, 
"Classifying User Requirements from Online Feedback in Small Dataset Environments using Deep Learning" 
in 29th IEEE International Requirements Engineering Conference (RE '21), Notre Dame, USA, 2021.

## Description of Artifact

This repository includes the following files and folders:

```
.
├── data/
├── models/
├── __init__.py
├── data_loader.py
├── evaluate.py
├── LICENSE.md
├── ML Baseline.ipynb
├── models.py
├── p1_train_with_bert.py
├── p1_train_with_elmo.py
├── p1_train_with_fasttext.py
├── p2_train_with_bert.py
├── p2_train_with_elmo.py
├── p2_train_with_fasttext.py
├── preprocessing.py
├── README.md
├── requirements.txt
├── train.py
└── utilities.py

2 directories, 17 files
```

### data/ directory
This directory contains two files, `P1-Golden.xlsx` and `P2-Golden.xlsx`, that were taken with permission from the dataset by Van Vliet et al. (available online at https://doi.org/10.5281/zenodo.3626185), and contain the gold standard for tasks P1 and P2 respectively.

### models/ directory
This directory contains a subdirectory `pre-trained`, which contains the pre-trained vector file used by our FastText model as well as `options` and `weights` for a pre-trained ELMo model. 
Apart from the pre-trained subdirectory, this directory also consists of fine-tuned BERT, ELMo and FastText models, which can be used to reproduce the results presented in our study. 

### __init__.py
This is an empty file that is needed to treat the directory containing it as a module.

### data_loader.py
This file consists of code corresponding to the data-loaders that we use for our models.

### evaluate.py
This file contains methods to evaluate trained models by making predictions on unseen data.

### LICENSE.md
This file contains the complete text of the Creative Commons by Attribution 4.0 license, under which this artifact is licensed.

### ML Baseline.ipynb
This jupyter notebook consists of code to reproduce results for the machine learning models used in our study, Naive Bayes and TF-IDF/SVM, for both tasks P1 and P2.

### models.py
This file consists of model definitions for BERT and ELMo models used in our study.

### p1_train_with_bert.py
This file can be used to train/fine-tune the BERT model for task P1 to reproduce the results in our study.

### p1_train_with_elmo.py
This file can be used to train/fine-tune the ELMo model for task P1 to reproduce the results in our study.

### p1_train_with_fasttext.py
This file can be used to train/fine-tune the FastText model for task P1 to reproduce the results in our study.

### p2_train_with_bert.py
This file can be used to train/fine-tune the BERT model for task P2 to reproduce the results in our study.

### p2_train_with_elmo.py
This file can be used to train/fine-tune the ELMo model for task P2 to reproduce the results in our study.

### p2_train_with_fasttext.py
This file can be used to train/fine-tune the FastText model for task P2 to reproduce the results in our study.

### preprocessing.py
This file consists of methods to pre-process text before it is used by different models.

### README.md
This file is the file you are currently reading.

### requirements.txt
This file contains various dependencies that need to be installed before Python can run various files in this project.

### train.py
This file consists of code to train a particular deep learning model.

### utilities.py
This file consists of some common utility methods used by other scripts.

## Installation Instructions

1. Make sure [Python 3.6+](https://www.python.org/downloads/) is installed. 
2. Install dependencies by running the command:
```
$ pip install -r requirements.txt 
``` 

## Steps to Reproduce

The results from our study can be reproduced by training the corresponding deep learning model (BERT, ELMo or FastText) using one of the aforementioned scripts with the name structure: `p<N>_train_with_<MODEL_NAME>.py` script.
For example, to train a BERT model for task P1, run this command:

```
$ python p1_train_with_bert.py 
```

These scripts will fine-tune a pre-trained model and produce an evaluation report for the corresponding model.