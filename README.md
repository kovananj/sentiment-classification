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


## Dataset

The dataset consists of approximately 4000 tweets labeled as positive (0) or negative (1). Ensure the dataset is placed in the `data/` directory with the filename `sentiment_tweets2.csv`.

