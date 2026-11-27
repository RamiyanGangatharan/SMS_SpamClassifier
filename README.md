# SMS Spam Classifier

A machine learning project built from scratch in Java to classify SMS messages as **Spam** or **Ham (Legitimate)** using the Multinomial Naive Bayes algorithm.

**Dataset:** [SMS Spam Collection – Kaggle](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset?resource=download)

**Objective:** Implement a machine learning classification algorithm without using prebuilt ML libraries. Learn the underlying mathematics, data processing, model training, and evaluation.

---

## 1. Project Setup

- [ ] Create Java project structure
- [ ] Define project requirements and scope
- [ ] Identify required Java libraries (if any)
- [ ] Download and inspect the dataset
- [ ] Understand the dataset's CSV structure and encoding

## 2. Dataset Management

- [ ] Design a representation for an SMS message
- [ ] Define an enum or equivalent representation for message classifications (HAM / SPAM)
- [ ] Implement dataset loading
- [ ] Handle CSV parsing and encoding
- [ ] Validate dataset records
- [ ] Handle missing or malformed records
- [ ] Count total messages
- [ ] Count spam messages
- [ ] Count legitimate messages
- [ ] Calculate class distribution percentages
- [ ] Identify duplicate messages
- [ ] Display dataset statistics and sample messages

## 3. Data Cleaning & Text Preprocessing

- [ ] Convert text to lowercase
- [ ] Remove or normalize punctuation
- [ ] Tokenize messages into individual words
- [ ] Handle whitespace and empty tokens
- [ ] Investigate and implement stop-word removal
- [ ] Handle repeated words and word frequencies
- [ ] Investigate whether stemming or normalization is necessary
- [ ] Apply consistent preprocessing to all messages
- [ ] Export preprocessed messages to a separate CSV file
- [ ] Verify preprocessing results using sample messages

## 4. Vocabulary & Feature Extraction

- [ ] Extract unique words from the training dataset
- [ ] Build a vocabulary
- [ ] Track total vocabulary size
- [ ] Count word occurrences across the dataset
- [ ] Track word frequencies separately for HAM and SPAM
- [ ] Determine how unknown words will be handled
- [ ] Export vocabulary and word-frequency statistics to CSV

## 5. Dataset Preparation

- [ ] Separate dataset into training and testing sets
- [ ] Use a reproducible random seed for splitting
- [ ] Ensure both sets contain representative HAM and SPAM samples
- [ ] Prevent duplicate messages from leaking between training and testing
- [ ] Ensure vocabulary and model statistics are derived only from training data

## 6. Naive Bayes Implementation

### 6.1 Class Priors
- [ ] Calculate HAM prior probability
- [ ] Calculate SPAM prior probability

### 6.2 Word Frequencies
- [ ] Calculate total word counts for each classification
- [ ] Calculate individual word frequencies for each classification

### 6.3 Conditional Probabilities
- [ ] Calculate word probabilities given HAM
- [ ] Calculate word probabilities given SPAM

### 6.4 Laplace Smoothing
- [ ] Understand the purpose of Laplace smoothing
- [ ] Implement smoothing for unseen words
- [ ] Experiment with different smoothing parameters

### 6.5 Log Probabilities
- [ ] Understand numerical underflow
- [ ] Implement log probability calculations
- [ ] Calculate combined classification scores

### 6.6 Prediction
- [ ] Implement model training
- [ ] Implement message classification
- [ ] Compare HAM and SPAM scores
- [ ] Return predicted classification
- [ ] Handle messages containing unknown words

## 7. Model Evaluation

- [ ] Generate predictions using the testing dataset
- [ ] Compare predictions against actual classifications
- [ ] Implement a confusion matrix
- [ ] Calculate accuracy
- [ ] Calculate precision
- [ ] Calculate recall
- [ ] Calculate F1 score
- [ ] Analyze false positives and false negatives

## 8. External Dataset Testing

- [ ] Find a second SMS spam dataset
- [ ] Inspect its structure and classification labels
- [ ] Prepare it using the same preprocessing pipeline
- [ ] Ensure no external test messages were used during training
- [ ] Evaluate the trained model against the external dataset
- [ ] Compare external testing results with original testing results
- [ ] Document differences in model performance

## 9. Experiments & Improvements

- [ ] Compare model performance with and without stop-word removal
- [ ] Experiment with different Laplace smoothing parameters
- [ ] Investigate the effect of class imbalance
- [ ] Compare different tokenization strategies
- [ ] Investigate the effect of duplicate messages
- [ ] Document experimental results and observations

## 10. Documentation

- [ ] Document project architecture
- [ ] Explain the Naive Bayes algorithm
- [ ] Document the mathematical formulas used
- [ ] Explain preprocessing decisions
- [ ] Document model evaluation results
- [ ] Record limitations and potential improvements
- [ ] Provide instructions for running the application

---

## Project Constraints

- Implement the Naive Bayes algorithm from scratch.
- Do not use prebuilt machine learning libraries.
- Implement probability calculations, smoothing, and prediction independently.
- Use Java's standard library for mathematical operations and data structures.
- External libraries may be used for non-ML utilities such as CSV parsing.
- Prioritize understanding the mathematics and algorithms over achieving high accuracy.