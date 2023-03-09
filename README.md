# NLP Engineer Assignment
## Assignment: Text Classification using Hugging Face

Definition & Scope of the problem statement

    Goal: Build a text classification model using the Hugging Face library to classify each document into one of multiple categories.
    Dataset: text documents
    Model: fine-tuned from a pre-trained language model such as BERT or GPT-2
    Evaluation: held-out test set

Experimental setup

    Dataset: IMDb dataset for sentiment analysis with 50,000 movie reviews labeled as either positive or negative.
    Steps:
        Data preprocessing
        Fine-tuning a pre-trained language model
        Model evaluation

Explanation of the measurements/metrics used

    Accuracy: Proportion of correctly classified instances over the total number of instances
    Precision: Proportion of true positives over the total number of instances classified as positive
    Recall: Proportion of true positives over the total number of positive instances
    F1 score: Harmonic mean of precision and recall

Flowchart/workflow of the experiments

    Load and preprocess data
        Load text data and labels
        Clean and tokenize text data
        Convert labels into numerical form
    Fine-tune pre-trained language model
        Load pre-trained language model
        Define and compile classification model
        Train classification model on preprocessed data
    Evaluate model performance
        Load held-out test set
        Predict labels for test set using trained model
        Compute accuracy, precision, recall, and F1 score
        Test with a pipeline example

Methodology

    Pre-trained language model: DISTILBERT-BASE-UNCASED
    Architecture diagram:
        6 layers
        768 hidden units
        12 self-attention heads
    Pre-training: English Wikipedia and BooksCorpus using masked language modeling (MLM) objective.
    Uncased variant: trained on lowercased text, treats uppercase and lowercase letters as the same.
    Advantages of pre-trained language model: significantly reduce the amount of data required for fine-tuning a text classification model.

Results

    Evaluation metric: Accuracy
    Accuracy measures the proportion of correctly classified instances over the total number of instances in a dataset.
