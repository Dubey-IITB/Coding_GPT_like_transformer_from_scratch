# GPT from Scratch: Mid-Term Progress Report

This repository contains the implementation of a Generative Pre-trained Transformer (GPT) model, following Andrej Karpathy's "Let's build GPT" tutorial.

## 📌 Project Status: Mid-Term Submission
**Current Progress:**
- Implemented data loading and preprocessing (TinyShakespeare dataset).
- Built a **Bigram Language Model** as a baseline architecture.
- Implemented the training loop, batching, and loss estimation.
- Generated initial text (currently non-sensical, as expected from a simple Bigram model).

**Video Milestone:** Completed up to timestamp **42:00**.

## 🛠️ Model Architecture (Current)
At this stage, the model predicts the next character based solely on the current character. It establishes a lower-bound performance baseline before the introduction of Self-Attention.

- **Token Embedding Table:** Maps characters to vector embeddings.
- **Optimization:** Uses AdamW optimizer.
- **Loss Function:** Cross-Entropy Loss.
- **Context:** Currently looks at a context window of size 1 (Bigram).

## 📂 Files
- `GPT_Implementation.ipynb`: The Jupyter notebook containing the source code, training loop, and generation output.
- `input.txt`: The TinyShakespeare dataset used for training (downloaded within the notebook).

## 🚀 Usage
To run this notebook:
1. Open the `.ipynb` file in Google Colab or Jupyter Notebook.
2. Run all cells to download the dataset, train the Bigram model, and see the loss decrease.
3. The final cell generates text based on the trained weights.

## 🔗 References
- [Andrej Karpathy: Let's build GPT: from scratch, in code, spelled out.](https://www.youtube.com/watch?v=kCc8FmEb1nY)
