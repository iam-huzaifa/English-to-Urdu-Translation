# English to Urdu Neural Machine Translation

## Overview

This project implements an **English to Urdu Neural Machine Translation (NMT)** system using the **Encoder-Decoder architecture** with deep learning. The model is trained to translate English sentences into Urdu by learning the relationship between source and target language sequences.

The primary objective of this project is to explore sequence-to-sequence learning for machine translation and understand the challenges of translating between English and Urdu.

---

## Features

- English to Urdu sentence translation
- Encoder-Decoder (Seq2Seq) architecture
- Data preprocessing and tokenization
- Vocabulary creation for both languages
- Model training and evaluation
- Translation inference on new English sentences

---

## Model Architecture

The project uses a **Sequence-to-Sequence (Seq2Seq)** model consisting of:

- **Encoder**
  - Embedding Layer
  - LSTM Encoder
- **Decoder**
  - Embedding Layer
  - LSTM Decoder
  - Dense Output Layer with Softmax

The encoder converts the input English sentence into a context vector, and the decoder generates the corresponding Urdu translation word by word.

---

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Dataset

The model was trained on an English–Urdu parallel dataset containing paired sentences.

### Data Preprocessing

- Lowercasing English text
- Tokenization
- Padding sequences
- Vocabulary generation
- Train-test split

---

## Training

The model was trained using:

- Loss Function: Sparse Categorical Crossentropy
- Optimizer: Adam
- Encoder-Decoder (LSTM)
- Teacher Forcing during training

---

## Results

The current model achieved an approximate **40% translation accuracy**.

Although the accuracy is relatively low for production use, the project successfully demonstrates the implementation of a basic Neural Machine Translation system using an Encoder-Decoder architecture.

Some translation outputs are meaningful, while others contain grammatical or contextual errors due to dataset limitations and the absence of an attention mechanism.

---

## Limitations

- Accuracy is around **40%**
- No Attention mechanism
- Limited training dataset
- Difficulty translating long and complex sentences
- Out-of-vocabulary (OOV) words reduce translation quality

---

## Future Improvements

Future work may include:

- Implementing **Bahdanau or Luong Attention**
- Using **Bidirectional LSTM**
- Training on a larger English-Urdu dataset
- Applying **Byte Pair Encoding (BPE)** or **SentencePiece**
- Hyperparameter tuning
- Using **Transformer architecture**

---

## Installation

```bash
git clone https://github.com/iam-huzaifa/English-to-Urdu-Translation.git

cd English-to-urdu-Translation

pip install -r requirements.txt
```

## Conclusion

This project demonstrates the implementation of an Encoder-Decoder based Neural Machine Translation system for English to Urdu translation. While the current model achieves approximately **40% accuracy**, it provides a strong foundation for understanding sequence-to-sequence learning and can be significantly improved by incorporating attention mechanisms, larger datasets, and modern Transformer-based architectures.

---


## License

This project is licensed under the MIT License.
