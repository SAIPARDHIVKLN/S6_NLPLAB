# NLP Laboratory

Python programs for the Natural Language Processing (NLP) Laboratory, organised into six experiments. Each program is a separate, independently runnable `.py` file containing the code followed by its expected output as comments.

## Experiments

| No. | Experiment | Programs |
|-----|------------|----------|
| 1 | Word Analysis | 11 |
| 2 | Word Generation | 12 |
| 3 | Morphology | 7 |
| 4 | N-Grams | 5 |
| 5 | Laplace Smoothing in N-Gram Language Model | 1 |
| 6 | POS Tagging (HMM) | 1 |

## Folder Structure

```
NLP-Lab/
├── README.md
├── requirements.txt
├── Experiment-1/
│   ├── Program-1.py   (Word Tokenization)
│   ├── Program-2.py   (Sentence Tokenization)
│   ├── Program-3A.py  (Stop Word Removal)
│   ├── Program-3B.py  (Print Stop Words in English)
│   ├── Program-4.py   (Word Frequency Analysis)
│   ├── Program-5.py   (Regular Expression Word Extraction)
│   ├── Program-6.py   (Word Length Analysis)
│   ├── Program-7.py   (Vocabulary Analysis)
│   ├── Program-8.py   (Character Analysis)
│   ├── Program-9.py   (Lexical Diversity)
│   └── Program-10.py  (Multilingual Word Analysis)
├── Experiment-2/
│   ├── Program-1.py ... Program-6.py              (main programs)
│   ├── Inflect-Program-1.py ... Inflect-Program-5.py  (inflect library)
│   └── Pattern-Verb-Conjugation.py                (pattern library, optional)
├── Experiment-3/
│   ├── Program-1.py   (Stemming)
│   ├── Program-2.py   (Lemmatization)
│   ├── Program-3.py   (POS-based Lemmatization)
│   ├── Program-4.py   (Morphological Analysis)
│   ├── Program-5.py   (Prefix & Suffix Identification)
│   ├── Program-6.py   (Inflectional Analysis)
│   └── Program-7.py   (Derivational Analysis)
├── Experiment-4/
│   └── Program-1.py ... Program-5.py
├── Experiment-5/
│   └── Program-1.py
└── Experiment-6/
    └── Program-1.py
```

## Python Requirements

- Python 3.9 or higher
- nltk
- inflect
- spacy (with the `en_core_web_sm` model)
- pattern (optional, only for two programs)

## Installation

```bash
pip install -r requirements.txt
python -m spacy download en_core_web_sm
```

NLTK data (`punkt`, `punkt_tab`, `stopwords`, `wordnet`) is downloaded automatically by the programs that need it. To download everything in advance:

```bash
python -m nltk.downloader punkt punkt_tab stopwords wordnet
```

Additional resources required by particular programs:

| Program | Requirement |
|---------|-------------|
| Experiment-1: Program-1, 2, 3A | NLTK `punkt`, `punkt_tab` (3A also `stopwords`) |
| Experiment-1: Program-3B | NLTK `stopwords` |
| Experiment-2: Inflect-Program-1 to 5 | `inflect` |
| Experiment-2: Pattern-Verb-Conjugation | `pattern` (optional) |
| Experiment-3: Program-2, 3 | NLTK `wordnet` |
| Experiment-3: Program-6 | spaCy model `en_core_web_sm` |
| Experiment-3: Program-7 | `pattern` (optional) |
| Experiment-4: Program-1 to 5 | NLTK `punkt`, `punkt_tab` |

## Running Programs

Run any program from the project root:

```bash
python Experiment-1/Program-1.py
python Experiment-3/Program-3.py
python Experiment-5/Program-1.py
```

Programs that ask for input will prompt in the terminal. A sample input and its output are given as comments at the bottom of each file.
