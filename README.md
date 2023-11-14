# Text Classifier Readme

This is a simple text classification demo using Streamlit. The application is designed to classify news headlines into predefined categories (tech, business, sports, entertainment, politics) using a Multinomial Naive Bayes classifier trained on the BBC News dataset.

## Prerequisites

Before running the application, make sure you have the following dependencies installed:

pip install pandas streamlit scikit-learn

## How to Run

1. Save the provided code in a Python file, e.g., `text_classifier_app.py`.
2. Download the [BBC News dataset](http://mlg.ucd.ie/files/datasets/bbc-fulltext.zip) and extract the contents to the same directory as the Python file.
3. Open a terminal and navigate to the directory where the file is saved.
4. Run the Streamlit application:

streamlit run text_classifier_app.py

5. The application will open in your default web browser.

## Usage

1. Enter the text you want to classify in the text area.
2. Click the "Predict" button to see the predicted category.

## Model Training

The Multinomial Naive Bayes classifier is trained on the BBC News dataset. The dataset is loaded from the `bbc-text.txt` file, and the text data is transformed using the `CountVectorizer`. The model is then trained and evaluated using the training and testing datasets.

## Notes

- The trained model is saved using the `pickle` library. This allows the application to load the model and make predictions on new text inputs.
- The application is designed to work with news headlines, and the categories are mapped as follows: 0 - TECH, 1 - BUSINESS, 2 - SPORTS, 3 - ENTERTAINMENT, 4 - POLITICS.
- Feel free to explore other text classification models or datasets to enhance the application further.

If you encounter any issues or have suggestions for improvement, please refer to the documentation for Streamlit and scikit-learn for assistance.
