# LSTM-Vs-simple-RNN-
LSTMs and RNN are old compared to LLMs, but still! this project by using PyTorch with RNNs, LSTMs, and a custom Seq2Seq model for English-to-French translation. Covers model creation, preprocessing, and training pipeline. Part 1 focuses on basic RNNs; Part 2 builds an end-to-end translation system. 
#  Neural Machine Translation using RNNs and LSTMs (English–French)

This repository showcases a two-part project implementing neural machine translation models using PyTorch. The goal is to build a sequence-to-sequence model capable of translating English sentences to French using LSTMs.

---

##  Project Structure

- **part_1_**: Introduction to RNNs, LSTMs, and basic language modeling.
- **part_2**: Full sequence-to-sequence pipeline for English–French translation.


##  Understanding RNN and LSTM

###  Recurrent Neural Networks (RNN)

Recurrent Neural Networks are designed for sequential data such as text or time series. Unlike feedforward networks, RNNs maintain a **hidden state** across time steps, allowing information to persist.

RNNs process one element of the sequence at a time while retaining memory of previous elements. This makes them ideal for tasks where **context** or **temporal ordering** is important.

**Limitations**:
- Suffer from the **vanishing gradient problem**, making it hard to learn long-term dependencies.
- Not effective when the relevant context is far from the current input.

---

###  Long Short-Term Memory Networks (LSTM)

LSTMs are an extension of RNNs designed to capture **long-term dependencies** in sequence data. They overcome RNN limitations by introducing:

- **Cell State** – acts as a conveyor belt for information flow.
- **Forget Gate** – decides what information to discard from the cell state.
- **Input Gate** – updates the cell state with new information.
- **Output Gate** – controls what part of the state is output to the next step.

LSTMs preserve information over longer sequences and are widely used in NLP, speech recognition, and time-series prediction.

---

###  RNN vs. LSTM: A Comparison

| Feature | RNN | LSTM |
|--------|-----|------|
| Structure | Simple loop | Gated memory unit |
| Memory | Short-term | Long-term and short-term |
| Handles vanishing gradient |  No |  Yes |
| Complexity | Lower | Higher |
| Performance on long sequences | Poor | Excellent |
| Training stability | Lower | Higher |
| Ideal Use Case | Simple sequence data | Translation, speech, complex NLP |
---

##  Features

###  Part 1
- Implements a **basic RNN** from scratch
- Constructs a general **LSTM model**
- Defines a custom LSTM class with PyTorch
- Tokenizes sample text
- Demonstrates forward propagation for sequence classification

###  Part 2
- Loads bilingual dataset (eng-fra.txt)
- Preprocesses and tokenizes English and French sentences
- Builds a custom `TranslationDataset` with PyTorch `Dataset`
- Defines an **Encoder-Decoder architecture** with LSTM units
- Uses teacher forcing during training
- Prints sample translations after training

---

## Libraries Used

- `PyTorch`
- `NLTK`
- `Pandas`
- `Torchtext` (optional if extended)
- `Torch.nn`, `torch.utils.data`

---

##  Dataset

The project uses a bilingual English–French sentence dataset (`eng-fra.txt`), where each line contains a sentence pair separated by a tab character.
## Author
Razieh Moradi Graduate Student, McMaster University  moradr1@mcmaster.ca
