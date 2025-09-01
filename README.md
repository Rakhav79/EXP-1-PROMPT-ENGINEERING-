# EXP-1-PROMPT-ENGINEERING-

## Aim: 
Comprehensive Report on the Fundamentals of Generative AI and Large Language Models (LLMs)
Experiment: Develop a comprehensive report for the following exercises:

Explain the foundational concepts of Generative AI.
Focusing on Generative AI architectures. (like transformers).
Generative AI applications.
Generative AI impact of scaling in LLMs.

## Algorithm:
The fundamental algorithm for a large language model based on the Transformer architecture can be broken down into a series of steps.

1.  **Tokenization:** The input text is broken down into numerical tokens (e.g., words, sub-words, or characters).
2.  **Embedding:** Each token is converted into a vector representation (embedding) that captures its semantic meaning. Positional encodings are added to these vectors to preserve the order of the words in the sequence.
3.  **Self-Attention:** The model calculates a "score" for each token to determine its relevance to every other token in the sequence. This is done through multi-head self-attention mechanisms, which allow the model to focus on different aspects of the input.
4.  **Feed-Forward Network:** The output of the attention layers is passed through a feed-forward neural network to further process the information.
5.  **Layer Normalization and Residual Connections:** These mechanisms are used throughout the model to stabilize the training process and ensure smooth information flow.
6.  **Decoding and Generation:** The model iteratively predicts the next token in the sequence based on the input and the tokens it has already generated. This process continues until a stop condition is met (e.g., the model generates an "end-of-sentence" token).
7.  Algorithm: Train Transformer-based LLM

Input:
  - Text corpus D (billions of tokens)
  - Vocabulary V
  - Hyperparameters: layers L, hidden size H, attention heads A

Output:
  - Trained Language Model M

Steps:

1. Data Preprocessing:
   a. Clean corpus (remove noise, duplicates).
   b. Tokenize text into subword units (Byte Pair Encoding or SentencePiece).
   c. Map tokens to embedding vectors.

2. Model Initialization:
   a. Initialize embedding matrix E ∈ R^(|V| x H).
   b. Apply positional encodings to preserve sequence order.
   c. Initialize L layers of transformer blocks:
      - Multi-Head Attention
      - Feedforward Networks
      - Residual + Layer Norm

3. Forward Pass:
   For each sequence in batch:
     a. Compute embeddings + positions.
     b. Pass through transformer layers.
     c. Predict next token probabilities using Softmax.

4. Loss Computation:
   - Use Cross-Entropy Loss:
     L = - Σ y_i log(p_i)

5. Backpropagation:
   - Compute gradients using chain rule.
   - Update weights with Adam optimizer.

6. Training Loop:
   - Repeat forward + backward pass until convergence.
   - Monitor validation perplexity.

7. Inference (Generation):
   a. Provide a prompt sequence.
   b. Predict next token iteratively.
   c. Use decoding strategies:
      - Greedy search
      - Beam search
      - Top-k or nucleus sampling

End.
This process is typically divided into a **pre-training phase** (training on massive, unlabeled datasets) and a **fine-tuning phase** (training on smaller, task-specific datasets to adapt the model for a particular use case).
## Output
 A comprehensive, multi-section report that explains the core concepts, architectures, applications, and scaling impacts of Generative AI and LLMs.Generative AI represents a paradigm shift in artificial intelligence. Its architectures — particularly transformers — have redefined what machines can generate. LLMs show remarkable abilities due to scaling laws, but they also introduce ethical, computational, and social challenges.

As we continue to scale and refine these models, the future will likely see AI systems that are more capable, creative, and aligned with human values — provided we manage their risks responsibly.

## Result
* **Foundational Concepts:** Generative AI is explained as the creation of new content by learning data patterns. This is distinct from discriminative AI.
* **Architectures:** The report details key architectures like GANs, VAEs, and, most importantly, Transformers, explaining the role of the self-attention mechanism.
* **Applications:** The report provides a broad overview of use cases across various fields, including content creation, software development, and science.
* **Scaling Impact:** The report outlines how increasing model size leads to predictable performance improvements, the emergence of new, unexpected abilities, and a significant increase in training costs.
* **Algorithm:** A simplified, step-by-step algorithmic breakdown of how a Transformer-based LLM processes and generates text is provided, from tokenization to decoding.
