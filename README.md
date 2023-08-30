# Using Deep Learning to Identify Sentiment in IMDb Movie Reviews

## 1. Introduction
- **Background**: Sentiment analysis, a pivotal task in Natural Language Processing, involves identifying the sentiment conveyed in a given piece of text, such as reviews for movies or products.
- **Objective**: The project introduces a deep learning model that combines Bidirectional Gated Recurrent Units (Bi-GRUs) with Convolutional Neural Networks (CNNs) to categorize movie reviews from IMDb as positive or negative based on their content.

## 2. Related Work
- **Deep Learning Models**: Various models, including CNNs, RNNs, LSTM networks, and GRU networks, have showcased promising results in sentiment analysis tasks.
- **Combination of CNNs and RNNs**: The fusion of CNNs and RNNs, such as GRUs and LSTMs, has been explored in the sentiment analysis literature.

## 3. Experimental Setup
- **Dataset**: Utilizes the IMDb movie reviews dataset sourced from Kaggle, consisting of 50,000 reviews evenly divided between positive and negative sentiments.
- **Preprocessing**: The dataset undergoes preprocessing steps like removal of HTML tags, special characters, URLs, email addresses, digits, and extra whitespace. Tokenization and case normalization are also applied.
- **Model Architecture**: The model commences with an Embedding layer using pre-trained Word2Vec embeddings, followed by Dropout, Bidirectional GRU, Batch Normalization, 1D CNN, and GlobalMaxPooling1D layers.

## 4. Results and Evaluation
- **Model Evaluation**: The model's performance is assessed using test accuracy and F1 score.
- **Comparison**: The Bi-GRU model slightly outperforms the LSTM model in test accuracy and F1 score, suggesting its better suitability for this task.

## 5. Conclusion and Future Work
- **Insights**: The Bi-GRUConv model exhibits superior performance compared to the LSTM model in terms of test accuracy and F1 score.
- **Future Directions**: Potential to explore architectural enhancements, evaluate scalability, and analyze the performance of models on different datasets and tasks.
