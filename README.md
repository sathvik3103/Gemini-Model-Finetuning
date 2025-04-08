# Gemini-Model-Finetuning

Fine Tuning 'gemini-1.5-flash-001' model on a newsgroups text dataset using the Parameter-efficient fine-tuning or PEFT technique.

## Overview

This project demonstrates how to fine-tune the `gemini-1.5-flash-001` model on a newsgroups text dataset using the Parameter-efficient fine-tuning (PEFT) technique. The notebook includes steps for data preprocessing, model tuning, and evaluation.

## Prerequisites

- Python 3.9 or above
- Jupyter Notebook
- Required Python libraries: `google-genai`, `dotenv`, `scikit-learn`, `pandas`, `email`, `re`

## Installation

To install the required libraries, run:

```bash
pip install google-genai python-dotenv scikit-learn pandas
```

## Dataset

The [20 Newsgroups Text Dataset](https://scikit-learn.org/0.19/datasets/twenty_newsgroups.html) contains 18,000 newsgroups posts on 20 topics divided into training and test sets.

## Notebook Contents

### 1. Introduction

The notebook starts with a title and a brief description of the task.

### 2. Library Imports and Version Check

Imports necessary libraries (`genai`, `types` from `google`) and checks the version of the `genai` library.

### 3. Setting up the API Client

Loads environment variables and sets up the API client using a Google API key.

### 4. Listing Models

Lists available models that support the `createTunedModel` action.

### 5. Dataset Description

Provides a description and a link to the 20 Newsgroups Text Dataset.

### 6. Loading the Dataset

Loads the 20 Newsgroups dataset into training and test sets and prints the list of class names.

### 7. Glimpse of the Dataset

Provides a glimpse of the dataset by printing the first data point.

### 8. Preparing the Dataset

Discusses the preprocessing steps and provides a function to preprocess the dataset. This includes removing personal information and structuring the text data.

### 9. Applying Preprocessing

Applies preprocessing to the training and test datasets and displays the first few rows of the processed training data.

### 10. Sampling the Data

Discusses sampling the data and provides a function to sample a specific number of rows per category.

### 11. Evaluating Baseline Performance

Discusses evaluating the baseline performance of the model and provides a function to predict the label of a sample post.

### 12. Prompt Engineering

Discusses using prompt engineering techniques to get better model responses and provides a function to generate content using the model.

### 13. Tuning a Custom Model

Discusses tuning a custom model and provides a function to tune the model using the training data.

### 14. Evaluation

Evaluates the tuned model and compares the predictions with the actual labels.

## Running the Notebook

To run the notebook, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/sathvik3103/Gemini-Model-Finetuning.git
   cd Gemini-Model-Finetuning
   ```

2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open the `Fine tuning.ipynb` notebook and follow the instructions provided in the cells.

## Conclusion

This project provides a comprehensive guide to fine-tuning the `gemini-1.5-flash-001` model using the PEFT technique on the 20 Newsgroups text dataset. It includes data preprocessing, sampling, evaluating baseline performance, tuning the model, and evaluating the tuned model.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The [scikit-learn](https://scikit-learn.org/) library for providing the 20 Newsgroups dataset.
- The [Google GenAI](https://github.com/google/genai) library for model tuning and evaluation.

For any questions or issues, please open an issue in the repository or contact the repository owner.
