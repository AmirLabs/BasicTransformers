# Positional Encoding in Transformers (PyTorch)

🚀 This project is a minimal implementation of **Positional Encoding** using PyTorch, a key component of Transformer-based models (like BERT, GPT, etc.).

## 🧠 What it does
The `PositionalEncoding` module adds information about the **position of tokens** in a sequence using sine and cosine functions of different frequencies — allowing the model to understand word order.

## 📦 Components
- `PositionalEncoding` class (subclass of `nn.Module`)
- Sinusoidal calculation for even and odd indices
- Shape: `(batch_size, seq_len, d_model)`
- Includes dropout for regularization

## 🔧 Example usage
```python
embedding = nn.Embedding(vocab_size, d_model)
pos_encoder = PositionalEncoding(d_model)

x = embedding(input_tokens)         # shape: (batch_size, seq_len, d_model)
x = pos_encoder(x)                  # adds positional info
```

## 🛠️ Requirements
- Python ≥ 3.7  
- PyTorch ≥ 1.10  
- math

## 📂 Structure
```
positional_encoding.ipynb     ← Main implementation notebook
README.md                     ← This file
```

## 📌 Inspired by
- "Attention is All You Need" (Vaswani et al., 2017)
- PyTorch official tutorials

---

Feel free to ⭐ the repo or fork for learning purposes!
