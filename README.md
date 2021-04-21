# Stroke Prediction

An analysis of stroke related health data. 
Dataset available on Kaggle at https://www.kaggle.com/fedesoriano/stroke-prediction-dataset

This repository contains a statistical exploration of the data, including t-testing, logit-testing and some visual diagrams. Further, we test the performance of XGBoost vs Regularized Logistic Regression in their ability to accurately classify stroke occurrence. 


## Requirements

A requirements.txt file is available in the repo. Use this file and pip to create your virtual environment using the following command through command prompt (or equivalent)

```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

## Results
As one would expect, XGBoost boasts superior performance, capturing 1.4% more of the true positive test class. However, the interesting part comes from the computational time, with XGBoost requiring an additional ~34 minutes to train and tune. The details of the training process and the results are stated in the research_paper.pdf file attached in the repo. 