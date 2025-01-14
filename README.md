# Sentiment Analysis with RNN Variants and Transfer Learning

### Contributors:
- **Alex Khoo Shien How** (U2220791B)
- **Leong Hong Yi** (U2120932C)
- **Lim Jun Hern** (U2120981B)
- **Ng Yong Jian** (U2120431E)
- **Oo Yifei** (U2120933E)

---

## Project Overview:
This project explores sentiment analysis using deep learning techniques, focusing on RNN-based models and enhancements. Key contributions include:
- Developing a baseline model using vanilla RNNs.
- Experimenting with variations like BiLSTM, BiGRU, and CNNs.
- Implementing advanced strategies like word embeddings, OOV handling, and transfer learning with RoBERTa.

---

## Methodology:
### 1. **Data Preprocessing**:
- Used Word2Vec GoogleNews embeddings.
- Applied tokenization, punctuation removal, case folding, and lemmatization using NLTK.
- Retained stopwords for context preservation.

### 2. **Model Variants**:
- **Vanilla RNN**: Tested aggregation methods (max pooling, mean pooling, MHSA).
- **BiLSTM & BiGRU**: Captured richer contexts through bidirectional processing.
- **CNN**: Extracted local patterns using convolutional filters.
- **BERT**: Provide content-based representation of text as feature extractor.

### 3. **Enhancements**:
- **Unfreezing Embeddings**: Enabled gradient flow for fine-tuning word embeddings.
- **OOV Handling**: Generated embeddings for OOV words using statistical methods.
- **Transfer Learning**: Leveraged pre-trained models (BERT, RoBERTa) for superior accuracy.

---

##  Key Findings:
- **Pooling Methods**: Max pooling consistently outperformed other aggregation strategies.
- **Transfer Learning**: RoBERTa outperformed all other models with a test accuracy of 88.74%.
- **OOV Handling**: Statistically generated embeddings effectively handled unseen words, improving accuracy.

---


## References:
- **Pre-trained Embeddings**: [Word2Vec GoogleNews](https://code.google.com/archive/p/word2vec/)
- **Transformer Models**: [Hugging Face Transformers](https://huggingface.co/)

---

## Acknowledgments:
This project was completed as part of the SC4002 Natural Language Processing module at Nanyang Technological University. Special thanks to our professor for guidance and insights.
