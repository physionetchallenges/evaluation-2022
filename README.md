# Scoring code for the George B. Moody PhysioNet/Computing in Cardiology Challenge 2022

This repository contains the Python and MATLAB evaluation code for the George B. Moody PhysioNet/Computing in Cardiology Challenge 2022.

The `evaluate_model` script evaluates the output of your classifier using the evaluation metric that is described on the [webpage](https://physionetchallenges.org/2022/) for the 2022 Challenge. While this script reports multiple evaluation metrics, we use the last score (`Challenge`) to rank your model.

## Python

You can run the Python evaluation code by installing the NumPy package and running the following command in your terminal:

    python evaluate_model.py labels outputs scores.csv class_scores.csv

where `labels` is a folder with labels for the data, such as the training database on the PhysioNet webpage; `outputs` is a folder containing files with your model's outputs ofr th edata; `scores.csv` (optional) is a collection of scores for your model; and `class_scores.csv` (optional) is a collection of per-class scores for your model.

## MATLAB

You can run the MATLAB evaluation code by installing Python and the NumPy package and running the following command in MATLAB:

    evaluate_model('labels', 'outputs', 'scores.csv', 'class_scores.csv')

where `labels` is a folder containing files with the labels for the data, such as the training database on the PhysioNet webpage; `outputs` is a folder containing files with outputs produced by your model for the data; `scores.csv` (optional) is a collection of scores for your model; and `class_scores.csv` (optional) is a collection of per-class scores for your model.

## Troubleshooting

Unable to run this code with your code? Try one of the [example classifiers](https://physionetchallenges.org/2022/#submissions) on the [training data](https://physionetchallenges.org/2022/#data). Unable to install or run Python? Try [Python](https://www.python.org/downloads/), [Anaconda](https://www.anaconda.com/products/individual), or your package manager.
