# Hemoglobin Prediction using Conjunctiva Images

## Team
Manas Satish Bedmutha <br>
Siddhant Saoji <br>
Jainish Nileshkumar Chauhan

## Introduction
This repository shows our initial experiments on using images of the conjunctiva to predict the Hemoglobin (Hb) levels of a person. Since Hb scores are the gold standard in determining anemia, and the threshold for anemia varies from region to region, we aim to assist medical professionals by giving them Hb scores so that they can make the best judgement. Our major aim is to provide accessibility to patients in remote areas where primary medical care cannot be reached instantly. This will help detect anemic patients in a timely manner and thus help save lives.

## Folder Structure

```
anemia-detection
│   README.md
│   requirements.text  
└───baselines
│   │   hue_score_svm.ipynb
│   └───mean_ann.ipynb 
└───docs 
└───experiments
│   │    vanilla_cnn.ipynb
│   │    visualize.ipynb
│   │    xgboost_linreg.ipynb
|   └───transfer-learning
|   |   |   learning.ipynb 
|   |   └───training.ipynb 
```

## Prerequisites
The dependencies are listed under requirements.txt and are all purely python based. To install them simply run
```
pip install -r requirements.txt
```

## Dataset
This repository uses the [Eyes-defy-Anemia](https://ieee-dataport.org/documents/eyes-defy-anemia) dataset for all the study and analysis. It also uses [HAM 10000](https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000) for the transfer learning priors.

## Running
Each notebook primarily uses four files, X_italy, X_india, y_italy and y_india which represent the masks and labels for each country. Simply changing path to the local folder containing the images and excel files will help run the files.
