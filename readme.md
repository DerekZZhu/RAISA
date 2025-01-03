# RAISA
The **Recordkeeping and Information Security Administration** is in charge of handling the copious amounts of data and reports from discovered anomalies around the globe. Each reported anomaly is classified by foundation scientists as either Safe, Keter, or Euclid.

## AIC
Artificially intelligent constructs (**AICS**) have been serving the foundation for years. This repository serves as an attempt to produce such an AIC for the goal to classify and tag SCP reports

## Structure
Data reports can be found in the repo and weights can be found in the weights section below, as they are very large, they have been uploaded to Huggingface to save space.

## Weights
https://huggingface.co/DerekZ/SCP-Classifier - roBerta

## Data
Data is hosted [here](https://huggingface.co/datasets/DerekZ/SCP-Reports-CLEAN/tree/main) on huggingface. There are 3 main datasets\
1. data.csv - this is the dataset containing somewhat cleaned SCP reports though includes author metadata. It is stored in the format: item, class, report
2. data_3class.csv - this dataset is for the task of only 3 class classifications (**safe**, **euclid**, **keter**), where all **thaumiel** class objects have been reclassified as safe and all **esoteric** and **uncontained** class objects have been reclassified as **keter**
3. data_multiclass.csv - this dataset holistically contains duplicate reports for SCP objects that have multiple classes, for example (esoteric-class, keter). Also for objects that were classified but had their classifications updated at a later date.

## Results
