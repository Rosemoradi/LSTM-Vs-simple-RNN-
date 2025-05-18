# LSTM-Vs-simple-RNN-
LSTMs and RNN are old compared to LLMs, but still! this project by using PyTorch with RNNs, LSTMs, and a custom Seq2Seq model for English-to-French translation. Covers model creation, preprocessing, and training pipeline. Part 1 focuses on basic RNNs; Part 2 builds an end-to-end translation system. 
#  Neural Machine Translation using RNNs and LSTMs (English–French)

This repository showcases a two-part project implementing neural machine translation models using PyTorch. The goal is to build a sequence-to-sequence model capable of translating English sentences to French using LSTMs.

---

##  Project Structure

- **part_1_**: Introduction to RNNs, LSTMs, and basic language modeling.
- **part_2**: Full sequence-to-sequence pipeline for English–French translation.

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

