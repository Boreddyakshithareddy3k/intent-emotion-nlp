# Intent & Slot Understanding Engine for Conversational AI

This project implements a joint model for **intent classification** and **slot filling** using a BERT-based encoder. It is designed as a core language understanding module for conversational agents, chatbots, and voice assistants.

## Features

- Joint training of **intent classification** and **slot filling** tasks
- BERT-based encoder for robust language representations
- Configurable training pipeline with reproducible scripts
- Simple **Streamlit demo app** for interactive testing of utterances

## Tech Stack

- Python, PyTorch
- Hugging Face Transformers (BERT)
- Streamlit (demo UI)

## Training

Example training command (SNIPS dataset):

```bash
pip install -r requirements.txt

python run_jointBERT.py \
  --task snips \
  --model_type bert \
  --model_name_or_path bert-base-uncased \
  --do_train --do_eval
