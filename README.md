# Arithmetic Expression Solver using a Decoder-Only Transformer

This project trains a decoder-only transformer to solve nested arithmetic expressions, generating the full step-by-step reduction of parenthesized addition problems (e.g., `(1+2)+8=` → `(3+8)=11`). Starting from a small baseline handling single-digit, two-number cases, the model is scaled up via curriculum training across 15,000 steps to handle up to five operands and three-digit numbers. The architecture uses causal self-attention with learned positional embeddings, trained with AdamW, cosine learning-rate decay, and EMA weight averaging. Accuracy is benchmarked across operand-count and digit-width combinations, with the final model, its weights, and a command-line inference script submitted for grading.


# Course 

DS 542 Deep Learning for Data Science - Boston University 
