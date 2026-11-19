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

## Getting started

### Option 1: Google Colab

1. Open the notebook in this repository.
2. Or launch it directly in Google Colab: [Open Session 01 in Colab](https://colab.research.google.com/github/Ali-Rzp/Practical-NLP/blob/main/Session-01/NLP_Text_Processing_and_Analysis.ipynb).
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
