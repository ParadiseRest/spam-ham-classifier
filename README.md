# Spam-Ham Classifier

This project is a machine learning-based email classification system that identifies emails as either spam or ham (non-spam). It leverages the `Logistic Regression` model and `TF-IDF` vectorization for feature extraction.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Model](#model)
- [Evaluation](#evaluation)
- [Prediction](#prediction)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project aims to provide a simple yet effective way to classify emails as spam or ham. The dataset is pre-processed, balanced, and used to train a `Logistic Regression` model. The model is evaluated for its performance and can make predictions on new email data.

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/spam-ham-classifier.git
    ```
2. Navigate to the project directory:
    ```bash
    cd spam-ham-classifier
    ```
3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage
1. Ensure you have your dataset in the `dataset.csv` file.
2. Run the script to train the model and make predictions:
    ```bash
    python spam_ham_classifier.py
    ```

## Data
The dataset used in this project should be in CSV format with two columns: `Category` and `Message`. The `Category` column should contain labels 'spam' or 'ham', and the `Message` column should contain the email text.

## Model
The model used in this project is `Logistic Regression`. The features are extracted using `TF-IDF Vectorization`.

## Evaluation
The model's performance is evaluated using `accuracy_score` and `classification_report` from `sklearn.metrics`.

## Prediction
To make predictions on new emails, simply pass the email text to the model's `predict` method after transforming the text using the `TF-IDF Vectorizer`.
