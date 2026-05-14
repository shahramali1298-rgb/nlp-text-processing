# 📚 NLP Text Processing Assignment
### Complete Pipeline: PDF Extraction → Preprocessing → Feature Extraction → Plotly Visualization

---

## 📄 Overview

This project demonstrates a **complete NLP text processing pipeline** applied to a real PDF document (*Frankenstein* by Mary Shelley — 280+ pages, public domain via Project Gutenberg).

The pipeline covers:
- PDF reading & text extraction
- Text preprocessing with **Regex-based cleaning**
- Feature extraction: **One Hot Encoding** & **TF-IDF**
- Interactive **Plotly** scatter plot visualization

---

## 📁 Repository Structure

```
nlp_assignment/
├── nlp_assignment.ipynb   ← Main Jupyter Notebook (all code)
├── requirements.txt        ← Python dependencies
└── README.md               ← This file
```

> **PDF Source:** *Frankenstein* by Mary Shelley  
> Downloaded automatically in the notebook from:  
> `https://www.gutenberg.org/files/84/84-pdf.pdf`  
> (Public Domain — Project Gutenberg)

---

## ⚙️ How to Run

### Option 1 — Local (Jupyter)

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/nlp-assignment.git
cd nlp-assignment

# 2. Install dependencies
pip install -r requirements.txt

# 3. Launch Jupyter
jupyter notebook nlp_assignment.ipynb
```

> Run all cells from top to bottom. The PDF will be downloaded automatically on first run.

### Option 2 — Kaggle Notebook

1. Go to [Kaggle](https://www.kaggle.com) → **Create Notebook**
2. Upload `nlp_assignment.ipynb`
3. Enable **Internet** in notebook settings
4. Click **Run All**

---

## 📦 Dependencies

```
PyMuPDF        # PDF reading (fitz)
nltk           # Tokenization, stopwords, stemming, lemmatization
scikit-learn   # One Hot Encoding, TF-IDF
pandas         # Tabular display
plotly         # Scatter plot visualization
requests       # PDF download
```

Install all at once:
```bash
pip install -r requirements.txt
```

---

## 🧪 Assignment Tasks Covered

| Section | Task | Status |
|---------|------|--------|
| Q1(a) | PDF Reading & Text Extraction | ✅ |
| Q1(a) | Total pages & sample text | ✅ |
| Q1(b) | Lowercase conversion | ✅ |
| Q1(b) | Remove numbers (Regex: `\d+`) | ✅ |
| Q1(b) | Remove special symbols (Regex: `[^a-z\s]`) | ✅ |
| Q1(b) | Remove extra spaces (Regex: `\s+`) | ✅ |
| Q1(b) | Remove punctuation | ✅ |
| Q1(b) | Tokenization | ✅ |
| Q1(b) | Stop word removal + count | ✅ |
| Q1(b) | Valid word count | ✅ |
| Q1(b) | Stemming (Porter Stemmer) | ✅ |
| Q1(b) | Lemmatization (WordNet) | ✅ |
| Q1(c) | One Hot Encoding (tabular) | ✅ |
| Q1(c) | TF-IDF feature names + values (tabular) | ✅ |
| Q1(d) | Plotly scatter plot (TF-IDF scores) | ✅ |

---

## 🔍 Regex Patterns Used

| Purpose | Pattern | Description |
|---------|---------|-------------|
| Remove Numbers | `\d+` | Matches one or more consecutive digits |
| Remove Special Symbols | `[^a-z\s]` | Matches any character that is NOT a letter or space |
| Remove Extra Spaces | `\s+` | Matches one or more whitespace characters |

---

## 📊 Sample Outputs

- **Total Pages:** 280+  
- **Raw Tokens:** ~100,000+  
- **Stop Words Removed:** ~45,000+  
- **Valid Words:** ~55,000+  
- **TF-IDF Features:** 50 top terms  
- **Visualization:** Interactive Plotly scatter plot with bubble sizes ∝ TF-IDF scores  

---


## 👤 Author

**Student Name:** *Shahram Ali Raja *  
**Course:** Natural Language Processing  
**Submission Date:** *5/14/2026*
