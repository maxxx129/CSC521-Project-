# Positional Encoding in Transformers

CSC521 Research Project based on the paper "Attention Is All You Need".

## Project Overview

In this project, we implemented a simplified Transformer model in PyTorch to understand the role of positional encoding.

Transformers process tokens in parallel and do not inherently understand sequence order. Positional encoding is used to inject order information into token embeddings.

## Implementation

We implemented the following components:

- Token Embedding
- Sinusoidal Positional Encoding
- Self-Attention
- Multi-Head Attention
- Feed-Forward Network
- Residual Connections and Layer Normalization
- Causal Masking
- GPT-style Transformer block
- Tiny language model

## Experiment

We conducted an experiment by removing positional encoding from the model.

### Observation:
- The model still produces outputs
- However, it loses sequence order information
- It cannot distinguish token positions

This shows that positional encoding is essential for sequence understanding.

## Data

We used small synthetic token sequences and a tiny character-level dataset for demonstration purposes.

## Code Source

The code was implemented by our group in PyTorch.

We did not directly copy or modify code from the provided repositories

However, our implementation is inspired by:
- "Attention Is All You Need" (Vaswani et al.)
- Standard Transformer architectures

## Screenshots
- Positional encoding visualization
- Model outputs
- Experiment results

## Key Insight

Positional encoding does not directly model relationships. It enables attention to learn relationships by providing order information.
