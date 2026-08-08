# Part-of-Speech Tagging — NLP Lab

**Course:** ITAI 2373 — Natural Language Processing  
**Assignment:** Lab 05  
**Author:** Jason Trimble

---

## Overview

A hands-on exploration of Part-of-Speech (POS) tagging using **NLTK** and **SpaCy**, progressing from basic concepts to real-world applications including customer service sentiment analysis and tagger benchmarking.

## Problem

How do computers understand the grammatical roles of words? POS tagging is the foundation for search engines, voice assistants, autocorrect, and sentiment analysis. This lab explores how different taggers handle everything from textbook sentences to messy social media text.

## What I Built

A complete Jupyter notebook with two major sections:

### Part 1 — In-Class Exercises
- Basic POS tagging with NLTK and SpaCy
- Side-by-side comparison of Penn Treebank vs. Universal Dependencies tag sets
- Ambiguity exploration (e.g., "lead" as verb vs. noun, "bank" as financial vs. river)
- Tag set trade-off analysis

### Part 2 — Homework Lab
- **Messy text processing:** Speech transcripts, social media posts, informal language
- **Customer service analysis:** Sentiment scoring, urgency detection, problem categorization from call transcripts
- **Tagger benchmarking:** Speed and accuracy comparison across formal, informal, technical, and conversational text
- **Edge case analysis:** Famous ambiguous sentences, garden path sentences, social media tokens
- **Data visualizations:** Sentiment by category, emotional adjective frequency, urgency indicators, performance charts

## Tools & Concepts

| Category | Details |
|----------|---------|
| **Libraries** | NLTK, SpaCy, pandas, matplotlib, seaborn |
| **NLP Concepts** | Tokenization, POS tagging, Penn Treebank, Universal Dependencies, lemmatization |
| **Analysis** | Sentiment analysis, urgency detection, tagger benchmarking, error analysis |
| **Visualization** | Bar charts, multi-panel figures, comparative analysis |

## Key Results

- **SpaCy** provides more intuitive broad-category tags (DET, ADJ, NOUN, VERB); **NLTK** offers finer-grained Penn Treebank distinctions
- Informal text (slang, emojis, abbreviations) challenges both taggers — preprocessing is essential for production use
- Customer service transcripts can be analyzed for sentiment, urgency, and problem type using POS-based features
- NLTK is faster for simple tagging; SpaCy provides richer linguistic features for production pipelines

## Evidence

- Fully executed Jupyter notebook with all outputs visible
- Four data visualizations (sentiment, emotional adjectives, problem indicators, urgency)
- Written reflections on tool selection, real-world applications, limitations, and future learning

## How to Run

```bash
pip install nltk spacy matplotlib seaborn pandas
python -m spacy download en_core_web_sm
jupyter notebook L05_Trimble_Jason_ITAI2373..ipynb
```

---

[← Back to Portfolio](../../README.md)