# NanoGPT_built_GPT-style_Transformer_from_scratch

**GPT From Scratch (Mini GPT)**

This repository contains a from-scratch implementation of a GPT-style decoder-only Transformer, built by closely following and understanding Andrej Karpathy’s Neural Networks: Zero to Hero tutorial series.

The goal of this project is learning and clarity, not scale — every major component of GPT is implemented explicitly to understand how modern language models work internally.

**Project Overview**

Implemented a mini GPT language model using PyTorch

Trained on a small text dataset due to hardware constraints

Focused on understanding:

Self-attention

Transformer blocks

Autoregressive language modeling

The model is capable of generating coherent text samples after training

This project prioritizes architectural understanding over performance or size.

**Architecture Summary**

The model follows the standard decoder-only Transformer architecture used in GPT models:

Token Embeddings

Positional Embeddings

Masked Multi-Head Self-Attention

Feed-Forward Network (MLP)

Residual Connections

Layer Normalization

Linear projection to vocabulary

Cross-entropy loss for training

Autoregressive text generation

**Implementation Details**

Framework: PyTorch

Tokenizer: Character-level tokenizer

Model Size: Scaled-down GPT (mini-GPT)

Training Hardware: CPU / Google Colab (T4 GPU)

Dataset: Small text corpus (e.g., Tiny Shakespeare or similar)

Due to limited hardware, the model is intentionally kept small.
The architecture is identical to large GPT models, only scaled down.


**Learning Goals**

This project was built to deeply understand:

How self-attention works (Q, K, V)

Why attention is scaled by √dₖ

How causal masking enforces autoregression

Why residual connections and LayerNorm stabilize training

How GPT differs from encoder-based models like BERT

How modern LLMs reduce to repeated applications of next-token prediction
