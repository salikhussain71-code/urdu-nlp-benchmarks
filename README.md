# Urdu NLP Benchmarks

Baseline models for Urdu Named Entity Recognition, sentiment analysis, and text classification.

## Why

Urdu NLP lacks widely used baseline numbers the way English tasks have (GLUE, SQuAD, etc.). This repo builds and documents baseline results on Urdu tasks so future work — including PAKGOV-RAG — has something concrete to compare against.

## Tasks

### Named Entity Recognition
Fine-tuned XLM-RoBERTa on the UNER corpus, evaluated with entity-level F1 using `seqeval`, compared against an mBERT baseline.

### Sentiment Analysis
Three-class sentiment classifier (positive/negative/neutral) for Urdu social media text, including handling of Urdu-English code-switching, which is common in Pakistani online writing.

### Document Classification
Classifier for Pakistani government document types (FBR, HEC, NADRA, SECP, and others) — built as a component that feeds into PAKGOV-RAG.

## Results

| Task | Model | F1 |
|---|---|---|
| NER | mBERT | — |
| NER | XLM-R | — |
| Sentiment | TF-IDF + LogReg (baseline) | — |
| Sentiment | XLM-R | — |

*(filled in as experiments are completed)*

## Author

Salik Hussain — github.com/salikhussain71-code

## License

MIT
```
