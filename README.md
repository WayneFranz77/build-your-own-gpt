# Build Your Own GPT

A GPT-style Transformer Language Model implemented from scratch in PyTorch.

This project demonstrates the core building blocks behind modern Large Language Models (LLMs), including tokenization, embeddings, self-attention, multi-head attention, transformer blocks, language modeling, training, checkpointing, and text generation.

---

## Project Overview

This project follows the architecture introduced by the GPT family of models and recreates a miniature GPT using the Tiny Shakespeare dataset.

The implementation includes:

- Character-level tokenization
- Token embeddings
- Positional embeddings
- Masked self-attention
- Multi-head attention
- Feed-forward networks
- Transformer blocks
- Layer normalization
- Residual connections
- Next-token prediction
- Text generation
- Model checkpointing

---

## Architecture

```text
Input Tokens
      ↓
Token Embeddings
      ↓
Positional Embeddings
      ↓
Transformer Blocks
      ↓
Layer Normalization
      ↓
Language Modeling Head
      ↓
Vocabulary Probabilities
```

---

## Dataset

Dataset:

```text
Tiny Shakespeare
```

Source:

https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt

Dataset Size:

```text
~1.1 MB
```

Vocabulary Size:

```text
65 Characters
```

---

## Model Configuration

```python
batch_size = 16
block_size = 32

n_embd = 64
n_head = 4
n_layer = 4

dropout = 0.2

learning_rate = 1e-3

max_iters = 5000
```

---

## Results

Training Loss:

```text
4.37 → 1.77
```

Validation Loss:

```text
4.36 → 1.91
```

Parameter Count:

```text
209,729
```

---

## Sample Generated Text

```text
CORIANCE:

CLA:
Wry chevere suees
Hougar, will forrim?

SICLO:
Sters, lother plazciour, many dead
```

The model successfully learned:

- Dialogue structure
- Character naming conventions
- Word formation
- Shakespearean formatting
- Language patterns

---

## Project Structure

```text
build-your-own-gpt/
│
├── data/
│   └── tiny_shakespeare.txt
│
├── models/
│   └── gpt_shakespeare.pth
│
├── notebooks/
│   └── gpt_train.ipynb
│
├── outputs/
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

## Installation

Create and activate a virtual environment:

```powershell
python -m venv venv

.\venv\Scripts\Activate.ps1
```

Install dependencies:

```powershell
pip install -r requirements.txt
```

---

## Running the Project

Open the notebook:

```powershell
code .
```

Navigate to:

```text
notebooks/gpt_train.ipynb
```

Run all cells in order.

---

## Future Improvements

Planned enhancements include:

- Larger embedding dimensions
- More Transformer blocks
- Longer context windows
- GPU training
- Learning rate scheduling
- Temperature sampling
- Top-k sampling
- Logistics-domain fine-tuning

---

## Key Concepts Demonstrated

- Deep Learning
- PyTorch
- NLP
- Transformers
- GPT Architecture
- Self-Attention
- Multi-Head Attention
- Language Modeling
- Tokenization

---

## Author

Wayne Franz

AI Engineering Portfolio Project