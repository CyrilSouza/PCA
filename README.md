 # Travel Insurance Prediction

This code performs travel insurance prediction using a logistic regression model and principal component analysis (PCA) for feature transformation. It utilizes the scikit-learn library in Python.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

To use this code, you need to have Python 3 and the following libraries installed:

- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

You can install these libraries using pip:


## Usage

1. Clone this repository to your local machine or download the source code.
2. Make sure you have the required libraries installed (see Installation section).
3. Prepare your dataset in a CSV format similar to the provided "Travel.csv" file.
4. Modify the code as needed, such as changing the features or the target variable.
5. Run the code using a Python IDE or execute it in a Jupyter Notebook.

## Dataset

The dataset used in this code is stored in a CSV file named "Travel.csv". It contains information about individuals, including their age, employment type, annual income, family members, chronic diseases, frequent flyer status, whether they have ever traveled abroad, and travel insurance status.

Make sure your dataset follows a similar structure with appropriate column names and data types.

## Model Training and Evaluation

1. The code begins by loading the dataset using pandas' `read_csv` function.
2. It selects specific features and the target variable for training the model.
3. Categorical variables in the dataset are encoded using `LabelEncoder` from scikit-learn.
4. The dataset is split into training and testing sets using `train_test_split` from scikit-learn.
5. A logistic regression model is instantiated using `LogisticRegression`.
6. The model is trained on the training data using the `fit` method.
7. The model's accuracy on the test data is evaluated using `accuracy_score` from scikit-learn.
8. PCA is performed on the feature matrix using `PCA` from scikit-learn to transform the data.
9. The transformed data is split into training and testing sets.
10. Another logistic regression model is instantiated, this time using the transformed data.
11. The new model is trained on the training data and its performance is evaluated using `score`.

Feel free to modify the code to suit your specific requirements and experiment with different models or techniques.

## Results

The accuracy score for the logistic regression model on the original data was approximately 0.6415. When the data was transformed using PCA, the accuracy score for the logistic regression model improved slightly to approximately 0.6533.

Please note that these scores are specific to the provided dataset and may vary depending on the dataset and model configuration used.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License

This code is licensed under the [MIT License](LICENSE).
