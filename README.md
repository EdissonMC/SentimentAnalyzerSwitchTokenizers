# 🧠 FlexibleSentimentAnalyzer

This project is a flexible tool for sentiment analysis using transformer-based models from Hugging Face. The main goal is to evaluate and compare the performance of different tokenizers on the same sentiment classification task.

## 🚀 What It Does

- Classifies sentiment (positive, negative, neutral) in short texts.
- Allows switching between various tokenizers .
- Measures how different tokenizers impact model performance.
- Designed for quick experimentation and lightweight evaluation.

## 🛠️ Tech Stack

- `PyTorch` + `Transformers` (Hugging Face)
- `TorchText` (for custom tokenizer support)
- `Matplotlib` for basic visualizations
- `Pandas` for data manipulation
- Sample dataset: a small, manually-labeled sentence set

## 🎯 Motivation

Tokenizers play a critical role in NLP model performance, often underappreciated. This project was born out of curiosity to explore how different tokenization schemes affect the outcomes of a sentiment classification task — in a clean and modular way.

## 🧪 How to Use

1. Select a base model (default: `bert-base-uncased`).
2. Choose any compatible tokenizer.
3. Run the sentiment analysis on example sentences.
4. Observe results and compare performance across tokenizers.

> The code is modular and designed for easy extension with new models or datasets.

## 📈 Example Usage

```python
analyzer = FlexibleSentimentAnalyzer(model_name="bert-base-uncased", tokenizer_name="roberta-base")
analyzer.analyze("I really love this project!")
