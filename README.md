# CS362-Thai-Mobile-App-Notification-Classifier

## Overview

The Mobile Notification Filtering System is a project aimed at classifying mobile application notifications into two categories: "ham" (non-marketing, advertising related, etc.) and "spam" (marketing, advertising related, etc.). This project addresses the common issue of receiving mixed notifications, such as delivery status updates and marketing offers, from mobile applications.

## Motivation

In our everyday lives, we often encounter scenarios where important notifications, such as delivery updates or service alerts, are mixed with marketing or advertising messages. This can lead to user frustration and difficulty in prioritizing important information. The Mobile Notification Filtering System aims to alleviate this pain point by accurately classifying notifications and filtering out irrelevant marketing content.

## Dataset

The dataset used in this project contains two fields: "label" and "content". The "label" field indicates whether a notification is "ham" or "spam", while the "content" field contains the text of the notification. The dataset mainly consists of notifications in the Thai language, focusing on shopping, food delivery, and service-related applications.

## Preprocessing

Preprocessing of the dataset involves several steps to prepare the text data for classification. This includes handling Thai language behavior, such as removing acronyms and substituting dates with a generic placeholder ("date"). Additionally, stop words and non-Thai/alphanumeric characters are removed to streamline the feature set for modeling.

## Model

The Multinomial Naive Bayes (MNB) classifier is chosen as the model for this project due to its effectiveness in text classification tasks. The MNB classifier is trained using the processed dataset to learn the probability distributions of features given each class (ham or spam). During prediction, the classifier calculates the posterior probability of each class for a given notification, allowing it to classify the notification as either ham or spam.

## Related Libraries

- numpy==1.26.4
- pandas==2.2.1
- scikit-learn==1.4.1
- matplotlib==3.8.3
- pythainlp==5.0.1
- pickleshare==0.7.5

## Usage

To use the Mobile Notification Filtering System, follow these steps:

1. Clone the project repository from GitHub and navigate to the project directory.
```
git clone https://github.com/Chayakorn2002/CS362-Mobile-App-Notification-Classifier.git
cd CS362-Mobile-App-Notification-Classifier
```
2. Install the required libraries using 
```
pip install -r requirements.txt
```
3. Prepare dataset with "label" and "content" fields.

4. Preprocess the dataset using the provided preprocessing methods. 

5. Train the Multinomial Naive Bayes classifier using the preprocessed dataset. 

6. Use the trained classifier to classify new notifications into ham or spam categories. 

7. Evaluate the performance of the classifier using metrics such as accuracy and precision. 

## Contributors

- Chayakorn Chiensuwikarn ( 6410450117 )
