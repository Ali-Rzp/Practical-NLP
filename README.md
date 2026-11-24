# Practical NLP

A collection of hands-on Jupyter notebooks for learning Natural Language Processing through practical Python examples.

## Session 01 — Text Processing and Linguistic Analysis

The first notebook follows a small text corpus through a practical NLP workflow:

- Corpus creation and inspection
- Lowercasing
- Punctuation and special-character removal
- Sentence and word tokenization
- Stop-word removal
- Stemming and lemmatization
- Part-of-speech (POS) tagging
- Chunking and parsing
- WordNet hypernyms and hyponyms
- Regular expressions: pattern matching, extraction, substitution, groups, and validation
- A combined preprocessing pipeline

## Session 02 — Text Representation and Embeddings

The second notebook introduces common ways to represent words and sentences as numerical vectors:

- Bag of Words (BoW)
- TF-IDF
- One-Hot Encoding
- Word2Vec
- FastText and subword information
- Sentence embeddings with Sentence Transformers
- Cosine similarity for comparing sentence embeddings

[Open the Session 02 notebook](Session-02/NLP_Session_2_Embeddings_Very_Simple.ipynb) · [Open Session 02 in Google Colab](https://colab.research.google.com/github/Ali-Rzp/Practical-NLP/blob/main/Session-02/NLP_Session_2_Embeddings_Very_Simple.ipynb)

The Word2Vec and FastText examples use a deliberately tiny toy corpus to demonstrate the APIs; their similarity results are not meaningful representations of language.

## Getting started

### Option 1: Google Colab

1. Choose a session notebook from the sections above.
2. Open it in this repository or use its Google Colab link.
3. Run the cells from top to bottom.

### Option 2: Run locally

Use Python 3.10 or newer.

```bash
git clone https://github.com/Ali-Rzp/Practical-NLP.git
cd Practical-NLP
python -m venv .venv
```

Activate the environment, then install dependencies:

**Windows PowerShell**
```powershell
.venv\Scripts\Activate.ps1
pip install -r requirements.txt
jupyter notebook
```

**macOS / Linux**
```bash
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

The notebook downloads the required NLTK data packages (such as Punkt, stopwords, and WordNet) when the relevant cells run. An internet connection is required for the initial downloads.

## Repository structure

```text
Practical-NLP/
├── Session-01/
│   └── NLP_Text_Processing_and_Analysis.ipynb
├── README.md
└── requirements.txt
```

## Notes

- Run the notebook cells in order because later sections reuse objects and resources created earlier.
- The examples use English text and NLTK's English-language resources.
- Preprocessing choices are task-dependent; removing punctuation or stop words is not always appropriate for every NLP application.
