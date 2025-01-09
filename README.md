# Generative-AI-Apply-Lightweight-Fine-Tuning-to-a-Foundation-Model

# Overview
This project demonstrates the complete workflow of training and inference using a pre-trained model with Parameter-Efficient Fine-Tuning (PEFT) techniques in PyTorch and Hugging Face. The main objectives are to:

## Load and evaluate a pre-trained model.
## Fine-tune the model using a PEFT technique.
## Perform inference with the fine-tuned model and compare its performance to the original model.

# Project Workflow

## 1. Load and Evaluate a Pre-Trained Model
Select a pre-trained model suitable for a sequence classification task.
Load the model along with its tokenizer from the Hugging Face library.
Use a dataset from Hugging Face's datasets library to evaluate the model's initial performance on the classification task.

## 2. Parameter-Efficient Fine-Tuning (PEFT)
PEFT Technique: Use LoRA (Low-Rank Adaptation) or another compatible technique to fine-tune the model.
Configure a PEFT model by setting up the appropriate hyperparameters (e.g., learning rate, batch size, etc.).
Train the model on the chosen dataset for at least one epoch.
Save the fine-tuned model using Hugging Face's save_pretrained method.

## 3. Inference with the Fine-Tuned Model
Load the fine-tuned model using the appropriate PEFT model class.
Re-evaluate the model's performance on the same sequence classification task.
Compare the results of the fine-tuned model with the original pre-trained model.
