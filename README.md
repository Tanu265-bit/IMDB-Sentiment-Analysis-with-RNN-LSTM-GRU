# IMDb Sentiment Analysis using RNN, LSTM and GRU

## Description

This project performs **sentiment analysis on IMDb movie reviews** using Deep RNN, LSTM, and GRU models built with TensorFlow and Keras.

The goal is to classify movie reviews into two categories:

* **Positive**
* **Negative**

## Models Used

* Deep RNN
* Deep LSTM
* Deep GRU

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Pandas
* Matplotlib

## Dataset

The project uses the **IMDb Movie Reviews Dataset**, containing:

* **25,000 training reviews**
* **25,000 testing reviews**

The dataset is used for binary sentiment classification.

## Preprocessing

The following preprocessing steps were performed:

* Vocabulary size limited to **10,000 words**
* Maximum sequence length set to **100**
* Reviews converted into integer sequences
* Padding applied to make all sequences equal in length
* An **Embedding layer** used to convert word indices into dense vector representations

## Model Architecture

### Deep RNN

```text
Input
  ↓
Embedding
  ↓
SimpleRNN
  ↓
SimpleRNN
  ↓
Dense (Sigmoid)
  ↓
Positive / Negative
```

### Deep LSTM

```text
Input
  ↓
Embedding
  ↓
LSTM
  ↓
LSTM
  ↓
Dense (Sigmoid)
  ↓
Positive / Negative
```

### Deep GRU

```text
Input
  ↓
Embedding
  ↓
GRU
  ↓
GRU
  ↓
Dense (Sigmoid)
  ↓
Positive / Negative
```

## Results

The three deep learning models are trained and evaluated on the IMDb dataset for binary sentiment classification.

The models predict whether a given movie review expresses a **positive or negative sentiment**.

## Project Workflow

```text
IMDb Dataset
     ↓
Text Preprocessing
     ↓
Integer Encoding
     ↓
Padding
     ↓
Embedding
     ↓
RNN / LSTM / GRU
     ↓
Dense + Sigmoid
     ↓
Sentiment Prediction
```

## Future Improvements

* Hyperparameter tuning
* Add Dropout layers to reduce overfitting
* Use Bidirectional LSTM/GRU
* Compare model accuracy
* Generate confusion matrices
* Compare training time
* Experiment with different embedding dimensions
* Experiment with different sequence lengths

## Project Files

```text
IMDB-Sentiment-Analysis-RNN-LSTM-GRU/
│
├── imdb_sentiment_analysis_rnn_lstm_gru.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Conclusion

This project demonstrates how **Deep RNN, LSTM, and GRU architectures** can be used for natural language processing and sentiment classification.

It also provides a practical comparison of different recurrent neural network architectures for processing sequential text data.
