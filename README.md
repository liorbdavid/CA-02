# CA-02
Intro to Machine Learning class- Coputer Assignment 02 Spam Detection using Naive Bayes




Brief description:
A spam email detection using Naive Bayes Classification Algorithm. The program trains a model with a set of emails labeled as Spam/Not Spam, then tests the model on another set of emails, predicts the category of the emails, and compares the accuracy with the correct classification.

Code explanation:
Part 1- set up functions
The first part consists of two function definitions (creations). The first to create a dictionary of words with the 3000 most common words from the ‘train-mails’ poll of email files. The second to label each email from both folders ‘train-mails’ and ‘test-mails’ into Spam and Not Spam, creating X_train and y_train as well as X_test and y_test.
Part 2- train
Using the email content and label (X_train and y_train respectively) from the ‘train-mails’ folder in order to train the model using Naive Bayes algorithm.
Part 3-test
After the model is created using the X_test (emails content from ‘test-mails’) to test the model and predict the emails label as Spam or Not Spam (y_predict).
Part 4- performance (accuracy)
Using the y_predict (predicted labels for the emails from the test phase) and comparing it to the y_test (actual labels of these same emails) to determine the model accuracy. We looked at varying dictionary lengths to see how that impacted the accuracy, precision, and recall of the model.

Software: 
Python 3.x
Libraries: 
import os
import numpy as np
from collections import Counter
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score
from sklearn.metrics import confusion_matrix
Import pandas as pd
Import matplotlib.pyplot as plt

Data set: given by professor. 702 emails, 351 are Spam and 351 are Not Spam. In one folder ‘train-mails’ there are 442 emails (mixed spam and not-spam) and another folder ‘test-mails’ there are 260 emails (mixed spam and not-spam).

Instructions:
Download the code file and the data folder with all the email files provided by professor Arin Brahma. Save both under the same folder, and ensure you use the relative path names of the data folder location (edit this part if needed). However, don’t change the data folder and data file names. The Jupyter Notebook contains the entire code and logic for the spam classifier. Before running the program make sure you download the required package and import the needed libraries.

Authors: Riley Nickel, Taleen Barake, Lior Ben David

