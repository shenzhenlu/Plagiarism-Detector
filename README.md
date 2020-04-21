# Plagiarism-Detector
A plagiarism detector that examines an answer text file and performs binary classification deployed with Sagemaker

## Software
* Anaconda Distribution 2020.02
* Python 3.7.6
* Jupyter Notebook 6.0.3
* AWS SageMaker

## Dataset
This data is a slightly modified version of a dataset created by Paul Clough (Information Studies) and
Mark Stevenson (Computer Science), at the University of Sheffield. You can read all about the data collection 
and corpus, at [their university webpage](https://ir.shef.ac.uk/cloughie/resources/plagiarism_corpus.html). 

> **Citation for data**: Clough, P. and Stevenson, M. Developing A Corpus of Plagiarised Short Answers,
Language Resources and Evaluation: Special Issue on Plagiarism and Authorship Analysis, In Press. [Download]

## Outline
* Clean and pre-process the data
* Define features for comparing the similarity of an answer text and a source text, and extract similarity features
* Select "good" features, by analyzing the correlations between different features
* Create train/test `.csv` files that hold the relevant features and class labels for train/test data points
* Upload train/test feature data to S3
* Define a binary classification model and a training script
* Train the model and deploy it using SageMaker.
* Evaluate the deployed classifier.
