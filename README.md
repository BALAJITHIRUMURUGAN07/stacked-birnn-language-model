# stacked-birnn-language-model
Next-word prediction using Stacked Bidirectional LSTM on movie plot summaries built with TensorFlow and Keras in Google Colab.
# Language Modelling Using Stacked Bidirectional RNNs
## 🎬 Domain: Movie Plot Summary Generation

---

## 📌 Problem Statement
In natural language processing, predicting the next word in a
sequence is a fundamental task that powers applications such as
story generation and plot recommendation systems. This project
uses a Stacked Bidirectional LSTM to learn sequential patterns
from movie plot summary data by processing text in both forward
and backward directions.

---

## 🧠 Model Architecture
| Layer | Details |
|-------|---------|
| Embedding | vocab_size × 64 |
| BiLSTM Layer 1 | 128 units, return_sequences=True |
| Dropout | 0.3 |
| BiLSTM Layer 2 | 64 units |
| Dropout | 0.3 |
| Dense Output | vocab_size, softmax |

---

## ⚙️ Algorithm
- Step 1: Import Libraries
- Step 2: Load Movie Plot Dataset
- Step 3: Tokenize Text Data
- Step 4: Generate N-gram Input Sequences
- Step 5: Pad Sequences
- Step 6: Define Features and Labels
- Step 7: Build Stacked Bidirectional RNN Model
- Step 8: Train for 100 Epochs
- Step 9: Predict Next Word from Seed Phrase
- Step 10: Visualize Accuracy and Loss

---

## 📊 Result
```
Input : a young hero
Output: a young hero discovers hidden powers and saves the world

Input : a detective solves
Output: a detective solves a mysterious murder in a dark city

Input : an astronaut gets
Output: an astronaut gets stranded alone on a distant planet

Input : a spy uncovers
Output: a spy uncovers a dangerous conspiracy inside the government

Input : a time traveler
Output: a time traveler tries to fix mistakes from the past

Input : a retired agent
Output: a retired agent comes back for one final dangerous mission
```
![Output](output.png)
---

## 🛠️ Technologies Used
- Python 3
- TensorFlow / Keras
- NumPy
- Google Colab

