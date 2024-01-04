
```markdown
# Text Classification with Logistic Regression

This project contains a Python script for classifying whether a given sentence is the next sentence of a provided paragraph. It utilizes a logistic regression model trained on TF-IDF vectorized text data.

## Project Overview

The script `text_classifier.py` performs the following steps:
1. Loads training and test datasets.
2. Preprocesses the text data (cleaning and tokenization).
3. Vectorizes the text using TF-IDF.
4. Splits the data into training and validation sets.
5. Trains a logistic regression model.
6. Validates the model and prints the F1 score.
7. Predicts on the test set and generates a submission file.

## Installation

Before running the script, ensure you have Python installed on your system. Then, install the required packages using the following command:

```bash
pip install pandas scikit-learn
```

## Usage

To run the script, simply execute it with Python:

```bash
python text_classifier.py
```

Ensure the `train.csv` and `test.csv` files are located in the same directory as the script.

## Data

The datasets `train.csv` and `test.csv` should have the following columns:
- `ID`: Unique identifier for each entry.
- `Paragraph`: The paragraph text.
- `Sentence`: The sentence text.
- `Is_Next`: Binary label indicating if the sentence is the next sentence of the paragraph (only in `train.csv`).

## Model Details

- **Model**: Logistic Regression
- **Vectorizer**: TF-IDF with a maximum of 10,000 features.
- **Evaluation Metric**: Weighted F1 Score

## Results

After running the script, the model's performance will be printed to the console. The predictions for the test set will be saved in `submission.csv`, formatted according to the competition's submission guidelines.

## Contributing

Contributions, issues, and feature requests are welcome. Feel free to check [issues page](https://github.com/yourusername/text-classification-repo/issues) if you want to contribute.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
