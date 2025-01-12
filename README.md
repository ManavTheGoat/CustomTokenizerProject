# Custom Tokenizer Training for NLP Tasks

This project demonstrates how to train a custom tokenizer using the WordPiece model and integrate it with Hugging Face Transformers. The project utilizes the WikiText-2 dataset as a case study, showcasing the creation of a tokenizer tailored for natural language processing (NLP) tasks.

## Project Overview

In NLP tasks, tokenization is a critical preprocessing step. This project walks through:

- Training a WordPiece tokenizer with a custom vocabulary size.
- Saving and loading the tokenizer for reuse.
- Integrating the tokenizer into Hugging Face Transformers for downstream applications.

## Dataset

- **Name**: [WikiText-2](https://huggingface.co/datasets/wikitext)
- **Description**: A large-scale, high-quality corpus of English text extracted from Wikipedia.
- **Usage**: The dataset’s training split is used to train the tokenizer.
