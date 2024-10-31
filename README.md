# Email/SMS Spam Classifier 

This project is a **Spam Classification** app built with **Streamlit** that classifies email or SMS messages as **Spam** or **Not Spam**. The classifier uses **Natural Language Processing (NLP)** techniques, including **TF-IDF Vectorization** and a **trained machine learning model** for prediction. 

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Model Information](#model-information)
- [Technologies Used](#technologies-used)
- [License](#license)

## Overview
The app is designed to help users identify spam messages using an ML model trained on SMS and email message data. Messages are preprocessed, vectorized, and classified into "Spam" or "Not Spam."

![App Screenshot](Screenshot%202024-10-31%20180937.png)

## Features
- Real-time classification of SMS and email messages
- Text preprocessing (lowercasing, tokenization, stopword removal, and stemming)
- Deployed with Streamlit for interactive usage

## Installation
Follow these steps to run the project locally:

1. Clone the repository:
    ```bash
    git clone https://github.com/Aishjahan/EMAIL-SMS-spam-classifier.git
    cd EMAIL-SMS-spam-classifier
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Download the NLTK data:
    ```python
    import nltk
    nltk.download('punkt')
    nltk.download('stopwords')
    ```

4. Place `vectorizer.pkl` and `model.pkl` files in the project directory. *(Ensure they are in the same directory as `app.py`.)*

5. Run the Streamlit app:
    ```bash
    streamlit run app.py
    ```

## Usage
1. Open the Streamlit app in your browser at `http://localhost:8501`.
2. Enter the SMS or email message you want to classify in the text input field.
3. Click on "Predict" to classify the message as **Spam** or **Not Spam**.

## Model Information
- **Vectorizer**: TF-IDF Vectorizer (`vectorizer.pkl`)
- **Model**: Pre-trained ML model (`model.pkl`), using algorithms like Naive Bayes or Logistic Regression

## Technologies Used
- **Python**: Core programming language
- **Streamlit**: For deploying the web app
- **scikit-learn**: For machine learning models and vectorization
- **NLTK**: For NLP preprocessing

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
