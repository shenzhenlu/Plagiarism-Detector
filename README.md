# Plagiarism-Detector
A plagiarism detector that examines an answer text file and performs binary classification; labeling that file as either plagiarized or not, depending on how similar that text file is to a provided, source text.

## Software
- Anaconda Distribution 2020.02
- Python 3.7.6
- Jupyter Notebook 6.0.3
- AWS SageMaker

## Dataset
This data is a slightly modified version of a dataset created by Paul Clough (Information Studies) and
Mark Stevenson (Computer Science), at the University of Sheffield. You can read all about the data collection 
and corpus, at [their university webpage](https://ir.shef.ac.uk/cloughie/resources/plagiarism_corpus.html). 

> **Citation for data**: Clough, P. and Stevenson, M. Developing A Corpus of Plagiarised Short Answers,
Language Resources and Evaluation: Special Issue on Plagiarism and Authorship Analysis, In Press. [Download]

## Outline
1. Download the data.
2. Process / Prepare the data.
3. Upload the processed data to S3.
4. Train a RNN model.
5. Test the trained model by sending test data to it after deployment.
6. Deploy the model again for the web app
