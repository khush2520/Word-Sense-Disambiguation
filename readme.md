
# WSD (Word Sense Disambiguation) using ML Algorithms and Feature Engineering

This repo consists of two notebooks. Both implements Word Sense Disambiguation (WSD)  but on different datasets. `WSD_sem_cor+omsti.ipynb` uses only semCor dataset while `WSD_sem_cor+omsti.ipynb` uses semcor and omsti dataset. The code implements WSD using various machine learning algorithms and feature engineering techniques.  The WSD process involves disambiguating the meaning of words in context. The code compares the accuracy of different machine learning models and different features for this task.

## Prerequisites

- **Python Environment:** This code is written in Python. Ensure you have Python installed.
- **Libraries:** The code uses NLTK and Scikit-learn libraries. Install them using the package manager pip:

```bash
pip install nltk scikit-learn
```

## Usage

1. **Data Preparation:**

   - Ennsure the XML files (`semcor+omsti.data.xml`, `ALL.data.xml`) and corresponding gold key files (`semcor+omsti.gold.key.txt`, `ALL.gold.key.txt`) are available. This dataset can be downloaded from [http://lcl.uniroma1.it/wsdeval/training-data](http://lcl.uniroma1.it/wsdeval/training-data)
2. **Running the Code:**

   - The code best runs in google collab.

## Code Structure

- **Importing Libraries:** The code starts by importing necessary libraries like NLTK, Scikit-learn, and more.
- **Data Preprocessing:**
- - Extracting corpus and dividing it into sentences.
  - Processing XML files to generate a dataset.
  - Saving the dataset into a JSON file (`semcor+omstidataset.json`).
- **Word Sense Disambiguation:**
  - Processing test data.
  - Loading datasets and gold key files for training and testing.
- **WordNet Integration:** Integration with NLTK's WordNet to fetch senses and examples.
- **Algorithms and Comparison:**
  - Implementation of Naive Bayes, K-Nearest Neighbors (KNN), and Maximum Entropy (MaxEnt) classifiers.
  - Configuration setup for different features and algorithms.
  - Model evaluation and accuracy comparison.

## Functionality

The code performs the following tasks:

- Processes XML files to create a dataset.
- Splits the dataset for training and testing purposes.
- Integrates WordNet to fetch senses and examples.
- Implements and evaluates Naive Bayes, KNN, and MaxEnt algorithms for WSD.
- Compares the accuracy of these algorithms based on different feature configurations.

## Instructions

1. Ensure necessary XML files and gold key files are available.
2. Run the code and observe the accuracy comparison of various ML algorithms for WSD based on different feature engineering approaches.
