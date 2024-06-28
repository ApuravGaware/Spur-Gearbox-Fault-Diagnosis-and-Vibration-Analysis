# Spur-Gearbox-Fault-Diagnosis-and-Vibration-Analysis

The dataset used is Gearbox Fault Diagnosis Dataset.

Link to dataset: https://www.kaggle.com/datasets/brjapon/gearbox-fault-diagnosis

Gearbox Fault Diagnosis Dataset include the vibration dataset recorded by using SpectraQuest’s Gearbox Fault Diagnostics Simulator.
Dataset has been recorded using 4 vibration sensors placed in four different direction, and under variation of load from '0' to '90' percent. Two different scenario are included:
1) Healthy condition and
2) Broken Tooth Condition
There are 20 files in total, 10 for healthy gearbox and 10 from broken one. Each file corresponds to a given load from 0% to 90% in steps of 10%.

The filename structure is indicative of the contents of the file:

First character being "h" for the healthy gearbox, "b" for the gearbox with the broken tooth
Last 1-2 characters being the gearbox load (0-90) during the measurement
Between those pieces of information, each filename has the characters "30hz".

The "dataset.ipynb" file is used to merge all the 20 files, pre-process and clean the dataset, and genearate the "data.csv" file.
The newly created data.csv has the following columns:
1) Sensor1
2) Sensor2
3) Sensor3
4) Load
5) State

The State column in data.csv represents the condition of the gear, either Healthy(represented by 0) or Broken(represented by 1).

The "dataset.ipynb" file is used to train various supervised machine learning models like KNN, Logistic Regression, Linear Regression, Naive Bayes, Random Forest to accurately distinguish between healthy and broken tooth gearbox states using data.csv. The model accuracy of these algorithms are also compared.
