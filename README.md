# Fraud Detection Tool

## Overview

The Hospital Bill Legitimacy Checker is an AI-based tool that helps determine the legitimacy of a hospital bill using scanned images of the bill. The system extracts the hospital address, retrieves the address of the patient, and then estimates the distance between them to predict whether the claimed bill is legitimate or fake.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/MadhavJain0119/Distance-Fraud-Detection.git
```
3. Install the required dependencies:
```pip install -r requirements.txt```

## Features

- Extracts hospital address and patient address from scanned hospital bills.
- Retrieves geo-locations for both addresses using an external API.
- Estimates the distance between the hospital and the patient's address.
- Predicts whether the bill is legitimate or potentially fraudulent based on the distance.

## Model Architecture

The AI model is built using a combination of deep learning techniques and natural language processing. It uses a convolutional neural network (CNN) for image processing to extract text from the scanned bill image. The extracted text is then processed using natural language processing (NLP) techniques to identify the hospital and patient addresses.
Data Collection

The model was trained on a diverse dataset of scanned hospital bills, containing both legitimate and fraudulent cases. The dataset was collected from various sources and carefully annotated for the hospital and patient addresses.

## Evaluation

1. The model's performance was evaluated on a separate validation dataset to measure its accuracy and other relevant metrics.
2. Cross-validation techniques were employed to assess the model's generalization ability.


## Limitations

- The accuracy of the model depends on the quality and diversity of the training data.
- OCR errors and inaccuracies in address extraction may affect the model's performance.
- The model relies on external APIs for geolocation, which might introduce latency and dependency issues.
