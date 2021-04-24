# Stroke Prediction

An analysis of stroke related health data. 
Dataset available on Kaggle at https://www.kaggle.com/fedesoriano/stroke-prediction-dataset

This repository contains a statistical exploration of the data, including t-testing, logit-testing and some visual diagrams. Further, we test the performance of XGBoost vs Regularized Logistic Regression in their ability to accurately classify stroke occurrence. 

## Description
model-* notebooks contain code to train and tune learning algorithms
preprocessing.ipynb contains code to generate the processed data required for the models
significance-testing-logisticReg.ipynb and statistical-exploration.ipynb contain code performing statistical tests on the dataset 
report.pdf is the corresponding paper that was written, describing the experiment that was undertaken
requirements.txt contains the python packages required to run the entire repo

## Requirements

A requirements.txt file is available in the repo. Use this file and pip to create your virtual environment using the following command through command prompt (or equivalent)

```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

## Running the notebooks
The first notebook to run is the statistical exploration, this will walk you through how the data was analyzed and the statistical tests that were conducted. These notebooks are titled 'statistical-exploration.ipynb' and 'significance-testing-logisticReg.ipynb'. 

Next, prior to running any of the modelling notebooks you will have to run the preprocessing notebook, this will generate the processed dataset that the modelling notebooks need. 

## Results
As one would expect, XGBoost boasts superior performance, capturing 1.4% more of the true positive test class. However, the interesting part comes from the computational time, with XGBoost requiring an additional ~34 minutes to train and tune. The details of the training process and the results are stated in the research_paper.pdf file attached in the repo. 

Thank you for visiting my repo
