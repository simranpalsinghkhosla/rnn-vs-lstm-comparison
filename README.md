# rnn-vs-lstm-comparison
# LSTM Time Series Prediction

## Project Description

This project demonstrates the implementation of a Long Short-Term Memory (LSTM) neural network using TensorFlow and Keras for sequential data prediction. The model is trained on synthetic sine-wave data and learns temporal patterns to predict future values in a sequence.

The notebook also includes a comparison between a Simple Recurrent Neural Network (SimpleRNN) and an LSTM model, highlighting the improved ability of LSTMs to capture long-term dependencies in sequential data.

---

## Features

* Synthetic time-series data generation using sine waves
* Data preprocessing and sequence creation
* Implementation of SimpleRNN and LSTM models
* Model training and evaluation
* Performance visualization using loss and MAE curves
* Comparison of recurrent neural network architectures

---

## Project Structure

```text
LSTM_model.ipynb
README.md
```

---

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib

---

## Model Architecture

### LSTM Network

```text
Input Layer
     ↓
LSTM Layer (32 Units)
     ↓
Dense Layer (1 Unit)
```

The LSTM layer captures temporal dependencies in the sequence, while the Dense layer predicts the next value.

---

## Dataset

A sine-wave dataset is generated using NumPy.

### Input

A sequence of 10 consecutive values.

Example:

```python
[0.10, 0.20, 0.30, ..., 0.84]
```

### Target

```python
0.91
```

The model learns to predict the next value based on the previous sequence.

---

## Training Configuration

| Parameter        | Value               |
| ---------------- | ------------------- |
| Optimizer        | Adam                |
| Loss Function    | Mean Squared Error  |
| Metric           | Mean Absolute Error |
| Epochs           | 20                  |
| Batch Size       | 32                  |
| Validation Split | 20%                 |

---

## Results

The model successfully learns the underlying pattern of the sine-wave data and achieves low prediction error.

Performance is evaluated using:

* Training Loss
* Validation Loss
* Mean Absolute Error (MAE)

Visualization plots are included in the notebook to analyze model learning behavior.

---

## Learning Outcomes

Through this project, I gained practical experience with:

* Recurrent Neural Networks (RNNs)
* Long Short-Term Memory (LSTM) Networks
* Time-Series Prediction
* TensorFlow and Keras
* Sequence Data Processing
* Deep Learning Model Evaluation

---

## Future Enhancements

* Train on real-world stock market data
* Experiment with stacked LSTMs
* Add Dropout regularization
* Hyperparameter tuning
* Compare with GRU and Transformer models

---

## How to Run

1. Clone the repository

```bash
git clone <repository-link>
```

2. Install dependencies

```bash
pip install tensorflow numpy matplotlib
```

3. Open the notebook

```bash
jupyter notebook LSTM_model.ipynb
```

4. Run all cells sequentially.

---

## Author

**Simranpal Singh**

M.Tech (Artificial Intelligence)

Passionate about Machine Learning, Deep Learning, NLP, and Generative AI.
