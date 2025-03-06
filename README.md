# sms_spam_detector

## Overview
This project builds an SMS spam classifier using machine learning. It leverages TF-IDF vectorization and a Linear Support Vector Classifier (LinearSVC) to determine whether a message is spam or not. The classifier is deployed as a web app using Gradio.

## Features
- **Preprocessing**: Text messages are vectorized using TF-IDF.
- **Model Training**: A pipeline is built with TF-IDF and LinearSVC.
- **Prediction**: Given a new SMS, the model predicts whether it is spam or not.
- **User Interface**: A simple web app using Gradio for real-time classification.

## Dataset
The dataset used is loaded from `Resources/SMSSpamCollection.csv` and contains:
- **text_message**: The SMS content.
- **label**: Classification (spam or ham).

## Technologies Used
- Python
- Scikit-learn
- Pandas
- Gradio

## Model Pipeline
1. **Text Preprocessing**: Convert SMS messages into numerical representations using TF-IDF.
2. **Training the Model**:
   - **Classifier**: Linear Support Vector Classifier (LinearSVC).
   - **Train/Test Split**: 67% training, 33% testing.
3. **Making Predictions**:
   - User input is classified as "Spam" or "Not Spam" based on trained model.

## How to Run
1. Install dependencies:
   ```bash
   pip install pandas scikit-learn gradio
   ```
2. Run the script:
   ```bash
   python script.py
   ```
3. The Gradio web app will launch, allowing users to test SMS messages for spam classification.

## Improvements
- **Expand the dataset** for better generalization.
- **Use deep learning models** like LSTMs for more advanced text classification.
- **Improve preprocessing** by including stemming and removing special characters.



