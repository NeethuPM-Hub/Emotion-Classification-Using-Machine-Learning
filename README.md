# Emotion-Classification-Using-Machine-Learning

## Project Overview

This project focuses on classifying text comments into different emotion categories using Machine Learning and Natural Language Processing (NLP) techniques.

The objective is to identify emotions expressed in text and compare the performance of two machine learning algorithms: **Naive Bayes** and **Support Vector Machine (SVM)**.

The emotion categories in this dataset are:
- Anger
- Fear
- Joy

## Objectives

- Load and preprocess the text dataset.
- Clean text, tokenize words, and remove stopwords.
- Convert text into numerical features using TF-IDF.
- Train Naive Bayes and SVM classification models.
- Evaluate and compare model performance using standard evaluation metrics.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Natural Language Processing (NLP)
- TF-IDF Feature Extraction
- Jupyter Notebook / Google Colab

## Project Workflow

1. **Data Loading:** Load the dataset and inspect the text comments and emotion labels.
2. **Text Preprocessing:** Convert text to lowercase, remove URLs and HTML tags, tokenize text, and remove stopwords while preserving important negation words.
3. **Feature Extraction:** Use TF-IDF Vectorization with unigram and bigram features to convert text into numerical representations.
4. **Model Development:** Train Multinomial Naive Bayes and Linear Support Vector Machine models.
5. **Model Evaluation:** Compare the models using accuracy, precision, recall, and F1-score.

## Model Performance

The models were evaluated using an 80:20 train-test split.

| Metric | Naive Bayes | Support Vector Machine |
|---|---:|---:|
| Accuracy | 92% | 95% |
| Weighted F1-score | 92% | 95% |

Based on the evaluation results, **Support Vector Machine (SVM) performed better** than Naive Bayes on the test dataset.

## How to Run the Project

1. Clone or download this repository.
2. Open the Jupyter Notebook in Jupyter or Google Colab.
3. Upload the dataset file (`nlp_dataset.csv`) to the notebook's working directory.
4. Install the required libraries if they are not already available:

   ```bash
   pip install pandas scikit-learn
   ```

5. Run all notebook cells to preprocess the data, train the models, and evaluate their performance.

## Repository Contents

- `Emotion_Classification.ipynb` — Jupyter Notebook containing the implementation and evaluation.
- `nlp_dataset.csv` — Dataset file, if included in the repository.

## Conclusion

This project demonstrates how NLP preprocessing and TF-IDF feature extraction can be combined with machine learning algorithms for text-based emotion classification. The experimental results indicate that SVM achieved better classification performance than Naive Bayes on this dataset.
