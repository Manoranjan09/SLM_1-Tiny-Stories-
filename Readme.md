# Small Language Model (SLM) from Scratch — TinyStories

This project explores building a Small Language Model (SLM) from scratch using the TinyStories dataset. It follows the learning workflow from the Vizuara SLM tutorial and uses Google Colab for experimentation and training.

## Project Overview

The goal is to understand the fundamental components of language models, including tokenization, dataset preprocessing, transformer architecture, and next-token prediction.

## Technologies Used

- **Python** — Core programming language
- **Google Colab** — Cloud-based development and GPU access
- **PyTorch** — Model implementation and training
- **Hugging Face Datasets** — Loading the TinyStories dataset
- **tiktoken** — GPT-2 tokenization
- **NumPy** — Efficient storage and processing of token IDs
- **nanoGPT-inspired preprocessing** — Preparing binary training data

## Dataset

**TinyStories:** [roneneldan/TinyStories](https://huggingface.co/datasets/roneneldan/TinyStories)

TinyStories contains short, simple stories designed to explore the language-learning capabilities of small language models.

The dataset includes:
- `train` — Training examples
- `validation` — Validation examples

## Workflow

1. Load the TinyStories dataset from Hugging Face.
2. Tokenize the text using the GPT-2 tokenizer.
3. Convert token IDs into binary files.
4. Generate `train.bin` and `validation.bin`.
5. Load batches of token sequences for model training.
6. Train a transformer model to predict the next token.
7. Evaluate the model using validation data.

## Project Files

- `SLM_TinyStories.ipynb` — Google Colab notebook containing the implementation.
- `train.bin` — Binary file containing training token IDs.
- `validation.bin` — Binary file containing validation token IDs.
- `README.md` — Project documentation.

*Note: Binary files are generated during preprocessing and may not be committed to GitHub.*

## Hardware

Development and experimentation are performed using Google Colab. GPU availability depends on the runtime configuration and resource limits.

## Learning Objectives

- Understand tokenization and vocabulary.
- Learn how language models process token sequences.
- Understand training and validation datasets.
- Explore binary data storage using NumPy memory mapping.
- Learn the fundamentals of transformer-based language model training.
- Build a foundation for future SLM fine-tuning and AI assistant projects.

## Acknowledgements

- [Vizuara](https://www.vizuara.com/) — Learning resources and tutorial guidance.
- [nanoGPT](https://github.com/karpathy/nanoGPT) — Reference implementation for language model training and data preprocessing.
- [Hugging Face](https://huggingface.co/) — Dataset hosting and machine learning tools.

## Disclaimer

This is an educational project intended for learning and experimentation. The model's capabilities depend on its architecture, training configuration, and dataset.

---

**Status:** In Progress 🚀
