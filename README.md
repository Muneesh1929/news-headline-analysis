# 📰 News Headline Classification with RNN  
*Turning headlines into insights with deep learning.*


This project builds a deep learning–based text classification model to categorize news headlines into 50 categories using **Recurrent Neural Networks (RNNs)** and **Natural Language Processing (NLP)**.

## 🔹 Dataset
- Source: [News Category Dataset](https://www.kaggle.com/datasets/rmisra/news-category-dataset)  
- ~210,000 news headlines with categories, short descriptions, authors, and dates.

## 🔹 Approach
1. **Data Preprocessing**  
   - Cleaned and normalized text (lowercasing, regex cleaning).  
   - Encoded labels and tokenized text.  
   - Applied sequence padding for uniform input.  

2. **Model Architecture**  
   - Embedding Layer (300 dimensions)  
   - SimpleRNN (200 units, ReLU)  
   - Dense Layers (150 → 100 → Softmax over 50 categories)  

3. **Training**  
   - Optimizer: Adam  
   - Loss: Sparse Categorical Crossentropy  
   - Achieved **96%+ accuracy** after 15 epochs with batch size 512.  

4. **Prediction Examples**  
   - *“Food quality was very good” → HEALTHY LIVING*  
   - *“India vs Pakistan match India won by 129 runs” → THE WORLDPOST*  
   - *“XYZ party will win election in next year” → POLITICS*  

## 🔹 Tech Stack
- Python · Pandas · Scikit-learn  
- TensorFlow/Keras  
- Natural Language Processing (NLP)  
- Recurrent Neural Networks (RNNs)

---

✨ Feel free to explore the notebook and code. Contributions and suggestions are welcome!

