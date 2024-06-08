# Sentiment Classification with BERT

This repository contains a sentiment classification project using BERT (Bidirectional Encoder Representations from Transformers). The model is trained to classify tweets or short texts as positive or negative sentiments. Sentimental Analysis can be very useful to find out depression and cure it before someone gets into serious trouble.



## Project Structure

- `data/`: Directory containing the dataset file.
- `transformers_multi_label_classification.ipynb/`: Jupyter notebooks for exploratory data analysis and experiments. Containing the  training, model evaluation, and prediction scripts.
- `bert_sentiment_model.pth`: The trained BERT model.
- `README.md`: Project documentation.

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/kovananj/sentiment-classification.git
    cd sentiment-classification
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv .venv
    source .venv/bin/activate  # On Windows, use `.venv\Scripts\activate`
    ```

3. **Follow and run the codes in the jupyter notebook:**

The notebook could also be opened in Google Colab for a faster and easier training.
  

## Dataset

The dataset consists of approximately 4000 tweets labeled as positive (0) or negative (1). Ensure the dataset is placed in the `data/` directory with the filename `sentiment_tweets2.csv`.


## Interpretation and Validation

**Performance Evaluation**

- Training and Validation Loss: The training loss significantly decreased from epoch 0 to epoch 1, indicating the model effectively learned from the training data. 
- Accuracy and F1 Scores: Both accuracy and F1 scores are extremely high, suggesting that the model is performing exceptionally well on the validation dataset. This could indicate a strong model performance, but it might also suggest potential overfitting, especially considering the very high scores.

**Impact of Hyperparameter Choices**
- Learning Rate: The learning rate of 1e-05 allowed the model to learn at a controlled pace, preventing drastic updates that could destabilize training.
- Batch Sizes: The chosen batch sizes for training and validation were effective in providing sufficient gradient updates per epoch without overwhelming the GPU memory.
- Epochs: Training for 2 epochs was sufficient to achieve high performance metrics, avoiding potential overfitting from excessive training.

**Validation and Benchmarking**
To validate and benchmark the model's performance, the following methods were used:

- Confusion Matrix and Classification Report: These metrics were computed to assess the model’s performance in distinguishing between positive and negative sentiments.

- Comparative Analysis: The results were compared to human judgment to ensure the model's outputs were reasonable and aligned with expected sentiments.

The trained BERT model demonstrated high performance metrics on the validation dataset, achieving near-perfect accuracy and F1 scores. However, qualitative analysis of example predictions revealed some errors, suggesting room for improvement in real-world scenarios. Further validation with a diverse dataset and potential model fine-tuning might be necessary to ensure robust performance.

