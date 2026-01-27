# Shakespeare Text Generation — Recurrent Neural Network (RNN)

This project implements a **character-level Recurrent Neural Network (RNN)** using PyTorch to generate text based on the works of William Shakespeare. The task forms part of a structured deep learning exercise focused on modelling **sequential text data** using recurrent architectures.

This project represents my **first foray into text-based machine learning**, extending my experience with neural networks from numerical and image data into natural language processing.

![Portrait of William Shakespeare](256px-William_Shakespeare_by_John_Taylor_edited.jpg)

The Chandros portrait of William Shakespeare, Wikimedia Commons.

---

### What’s in this repository

- **Jupyter Notebook:** RNN implementation and training workflow (`shakespeare_task.ipynb`)  
- **Images:** visuals
- **Dataset:** `tiny_shakespeare.txt` 
- **Requirements:** Python dependencies (`requirements.txt`)  

---

### Project Context

Unlike traditional feedforward neural networks, text data is inherently sequential — meaning that context and order strongly influence meaning. Recurrent Neural Networks are specifically designed to address this challenge by maintaining an internal state that carries information forward through a sequence.

In this task, a simple RNN was trained on the **Tiny Shakespeare dataset**, a collection of text extracted from Shakespeare’s plays and sonnets. The objective was to build a character-level language model capable of predicting the next character in a sequence and generating new text based on learned patterns.

The task required:

- Preparing character-level sequences  
- Vectorising text using one-hot encoding  
- Building an RNN using PyTorch  
- Training the model for 10 epochs  
- Generating a sample of 100 words of text  

---

## Approach Overview

- Text preprocessing and character mapping  
- Sequence generation using sliding windows  
- One-hot encoding of input and target characters  
- Construction of a simple RNN architecture  
- Training using cross-entropy loss and the Adam optimiser  
- Evaluation using loss and perplexity metrics  
- Text generation from a seed sequence  

---

## Key Insights / Findings

- The model successfully learned basic character-level patterns such as spacing, punctuation, and common letter combinations.  
- Generated text exhibited limited semantic coherence, reflecting the constraints of a simple RNN architecture.  
- Loss values improved only marginally, indicating that additional training time and architectural refinement would be required for stronger performance.  
- This behaviour is consistent with known limitations of vanilla RNNs, particularly their difficulty in retaining long-range context.  

Overall, the results illustrate both the potential and limitations of early recurrent architectures in language modelling tasks.

---

## Skills Demonstrated

**Analysis**
- Text preprocessing and sequence construction  
- Interpretation of loss and perplexity metrics  

**Modelling**
- Character-level Recurrent Neural Networks  
- Sequential data modelling  
- Neural network training workflows  

**Evaluation**
- Model performance assessment using perplexity  
- Interpretation of generated text output  

**Tools**
- PyTorch  
- Python  
- NumPy  
- Jupyter Notebook  

---

## Requirements / How to Run

Install the required Python dependencies:

```bash
pip install -r requirements.txt
