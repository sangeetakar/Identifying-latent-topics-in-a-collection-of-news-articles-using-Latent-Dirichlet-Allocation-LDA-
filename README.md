# Identifying-latent-topics-in-a-collection-of-news-articles-using-Latent-Dirichlet-Allocation-LDA-

---

News Topic Modeling using LDA (NLP)

```markdown
# News Topic Modeling using LDA (Latent Dirichlet Allocation)

This project applies **Natural Language Processing (NLP)** and **unsupervised machine learning** to extract hidden topics from a large collection of news headlines using **Latent Dirichlet Allocation (LDA)**.

---

## 📌 Project Overview

- Dataset: UCI News Aggregator Dataset
- Articles: ~422,000 news headlines
- Categories: Business, Science, Entertainment, Health
- Goal: Discover hidden thematic structures in news data

---

## ⚙️ Workflow

### 1. Data Loading & Cleaning
- Loaded dataset from UCI repository
- Converted timestamps to datetime format
- Extracted temporal features (day, month, week)

---

### 2. Text Preprocessing
Performed NLP preprocessing using NLTK:

- Tokenization
- Stopword removal
- Lemmatization
- Removal of punctuation and noise

Output: Clean tokenized corpus

---

### 3. Feature Engineering
- Created **Bag-of-Words representation**
- Built dictionary using Gensim
- Filtered extreme words using:
  - min frequency threshold
  - max document frequency limit

---

### 4. Topic Modeling (LDA)
- Trained **Latent Dirichlet Allocation (LDA)** model
- Extracted:
  - 4 to 7 latent topics
- Topics included:
  - Finance
  - Technology
  - Health
  - Entertainment
  - Social Media

---

### 5. Prediction on New Data
- Applied trained LDA model to unseen headlines
- Assigned topic probabilities per headline
- Classified dominant topic per article

---

## 📊 Results

| Metric | Observation |
|--------|------------|
| Dataset size | ~422K headlines |
| Topics extracted | 7 |
| Model type | Unsupervised LDA |
| Output | Topic probability distribution |

---

## 📈 Exploratory Data Analysis

- Article distribution across categories
- Monthly and weekly publishing trends
- Publisher frequency analysis (Reuters, Huffington Post, etc.)
- Category imbalance visualization

---

## 🧠 Key Insights

- Financial and technology news dominate topic clusters
- LDA effectively separates semantic themes without labels
- Temporal patterns show clear publishing spikes across weeks/months
- Headlines are strong enough signals for topic inference

---

## 🛠️ Tech Stack

- Python
- NLTK
- Gensim
- Scikit-learn
- Pandas
- Seaborn / Matplotlib

---

## 📊 Visualizations

- Category distribution plots
- Weekly news trends
- Publisher frequency analysis
- Topic word distributions
- Line plots for temporal trends

---

## 🚀 How to Run

```bash
pip install nltk gensim scikit-learn pandas seaborn matplotlib
python lda_topic_modeling.py
