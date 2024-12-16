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

## Steps to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/CustomTokenizerProject.git
cd CustomTokenizerProject
```

### 2. Install Dependencies

Create a virtual environment (optional but recommended) and install the required Python libraries:

```bash
pip install -r requirements.txt
```

### 3. Run the Notebook

Launch Jupyter Notebook and open the `training-a-tokenizer.ipynb` file:

```bash
jupyter notebook training-a-tokenizer.ipynb
```

Follow the steps in the notebook to train and test the tokenizer.

## Key Highlights

1. **Configurable Tokenizer Training**:

   - Vocabulary size and special tokens are adjustable.
   - Utilizes the `Tokenizers` library for efficient WordPiece training.

2. **Dataset Handling**:

   - Loads WikiText-2 dataset using the Hugging Face `datasets` library.
   - Batches data for efficient tokenizer training.

3. **Integration with Hugging Face**:

   - Saves the trained tokenizer in Hugging Face format.
   - Reloads the tokenizer for downstream NLP tasks.

4. **Reproducibility**:

   - Includes logging for process tracking.
   - Configurations are stored in a dictionary for easy adjustments.

## Directory Structure

```
CustomTokenizerProject/
├── training-a-tokenizer.ipynb   # Main notebook for training the tokenizer
├── README.md                   # Project documentation
├── requirements.txt            # Python dependencies
├── tokenizer/                  # Saved tokenizer files
│   ├── config.json
│   ├── vocab.txt
│   ├── special_tokens_map.json
│   ├── tokenizer_config.json
├── .gitignore                  # Git ignore file
```

## Dependencies

- Python 3.8+
- `transformers`
- `datasets`
- `tokenizers`
- `logging`

To replicate the environment, use the `requirements.txt` file provided.

## Future Work

- Experiment with different tokenizer models (e.g., BPE, Unigram).
- Train tokenizers on other datasets.
- Fine-tune Hugging Face models using the trained tokenizer.


