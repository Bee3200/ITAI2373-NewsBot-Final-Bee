# ITAI2373-NewsBot-Final-Bee
Final Project — NewsBot Intelligence System 2.0 (ITAI 2373) — Solo

# ITAI2373-NewsBot-Final-Bee

**Course:** ITAI 2373  
**Project:** NewsBot Intelligence System 2.0 — Solo  
**Submitter:** Bryan T (solo)  
**Repository URL:** (this page)  
**Submission Tag:** v1.0.0

---

## 1) Executive Summary (What this does in plain English)
This project builds a news-category classifier using the BBC news dataset text. The pipeline cleans text, splits train/test with stratification, vectorizes with TF-IDF, trains linear models (Logistic Regression baseline), and reports accuracy and a per-class classification report. A small POS and VADER sentiment sample is included for qualitative insight.

**Key Result:** Logistic Regression reaches ~0.9+ accuracy on the held-out test set (exact value shown in notebook output and `reports/metrics.json` if exported).

---

## 2) How to run (exact steps)
You can run entirely in **Google Colab** (no local installs required).

1. Open **`ITAI_2373_NewsBot_Final.ipynb`** (in this repo).  
2. Click **Open in Colab** (or upload to Colab).  
3. In Colab: **Runtime ▸ Run all**.  
4. When prompted by NLTK the first time:
   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('vader_lexicon')
   nltk.download('universal_tagset')

