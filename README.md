# Swahili Language Model for Masked Word Prediction

This repository contains an implementation of a **Swahili language model** that predicts or completes a missing part of a sentence given the surrounding words.  

For example:  

**Input Text:**  
Wakati [MASK] leo.

The model might suggest the following completions:  
- Wakati, leo.  
- Wakati : leo.  
- Wakati ya leo.  
- Wakati wa leo.  
- Wakati na leo.  

## Model Details  

The model is fine-tuned using Hugging Face's Transformers library for **Masked Language Modeling (MLM)** tasks in Swahili.  

To replicate or use the model, you will need to download the **LLaMa3.2 1B model** from:  
[https://huggingface.co/meta-llama/Llama-3.2-1B](https://huggingface.co/meta-llama/Llama-3.2-1B)  

## Setup  

To set up the environment and dependencies, the following packages were installed:  
```bash
pip install keras==2.15.0
pip install tensorboard==2.15.0
pip install ml-dtypes==0.2.0
pip install transformers datasets torch sentencepiece
pip install tensorflow
pip install accelerate>=0.26.0
