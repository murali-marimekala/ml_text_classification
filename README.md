# Text Classification Project

This project demonstrates a simple text classification model using Python and scikit-learn. It trains a Multinomial Naive Bayes classifier on a dataset of text files and predicts labels for new text data.

## Implementation

The code is structured into four main steps:

1. **Load and Preprocess Data:** Reads text files from a specified folder, extracts their content, and infers labels from file names.
2. **Train a Model:** Uses TF-IDF vectorization to convert text into numerical features and trains a Multinomial Naive Bayes model.
3. **Save the Model:** Saves the trained model and vectorizer to disk using joblib for later use.
4. **Predict New Data:** Loads the saved model, vectorizes new text data, and predicts its label.

**Dependencies:**

- Python 3.x
- scikit-learn
- pandas
- joblib

**Usage:**

1.  **Data:** Place your training data text files (as zip file) in the `data` folder. The file names should follow the pattern `<label>_<unique_identifier>.txt`, where `<label>` represents the category or class of the text.
2.  **Training:** Execute the main script using the notebook (ipynp). The code will ask to load the data, choose upload and select training_data.zip to train the model.
3.  **Prediction:** Use the `predict_new()` function to predict labels for new text data by providing the data folder (predict_data.zip) path and the saved model and vectorizer.

## Data Folder Structure

The `data` folder contains the following:

-   **Training data:** Text files used for training the model. These files should be placed as zip file under `data` folder. Download these files before you run the notebook
-   **Prediction data:** Text files for which you want to predict labels. These can also be uploaded via `files.upload()` during runtime. Note that the predictions will be generated for the files within the zip file. 

 ## Contributing

Contributions are welcome! Please feel free to submit pull requests for bug fixes, enhancements, or new features.

## License

This project is licensed under the [MIT License](LICENSE).
