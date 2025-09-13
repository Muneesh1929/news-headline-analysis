Description:
Developed a deep learning–based NLP model to classify news headlines into categories using the News Category Dataset (~210K records). The project demonstrates the application of data preprocessing, word embeddings, and recurrent neural networks (RNNs) for text classification.

Key Steps & Contributions:

Data Preprocessing:

Loaded and cleaned ~210,000 news headlines with metadata.

Applied text normalization (lowercasing, regex-based cleaning) and label encoding for categorical targets.

Feature Engineering:

Tokenized and vectorized text sequences using Keras Tokenizer.

Padded sequences to ensure uniform input length.

Implemented Word2Vec-like embeddings via Keras Embedding layer.

Model Architecture:

Built a Sequential Deep Learning model with:

Embedding layer (300-dim vector space)

SimpleRNN (200 units, ReLU)

Dense layers (150 → 100 → 50 classes with Softmax)

Optimized using Adam optimizer and sparse_categorical_crossentropy loss.

Training & Performance:

Trained over 15 epochs with batch size 512.

Achieved 96%+ accuracy on training data, demonstrating strong text classification performance.

Prediction Examples:

“Food quality was very good” → HEALTHY LIVING

“India vs Pakistan match India won by 129 runs” → THE WORLDPOST (Sports/World)

“XYZ party will win election in next year” → POLITICS

Tech Stack: Python, Pandas, Scikit-learn, TensorFlow/Keras, NLP, RNN
