Preprocessing:
Implemented a custom PyTorch Dataset class. Images were resized and normalized; text was tokenized for both LSTM (GloVe embeddings) and BERT. Data augmentation was applied to address class imbalance. Sample memes, class distributions, and word clouds were visualized.

Late Fusion Models:
Built and trained multiple image-text combinations (CNN+LSTM, CNN+BERT, ResNet+LSTM, ResNet+BERT). Outputs were fused and passed to a final classifier. Models were evaluated using AUROC, accuracy, precision, recall, and F1-score.

Early Fusion Models:
Extracted intermediate features (BERT [CLS] tokens, ResNet features) and fused them early via a multi-layer perceptron. Also experimented with optional cross-modal attention.

Evaluation:
Used TensorBoard to track training loss, AUROC, and performance. Visualized confusion matrices and ROC curves. Final analysis included comparison of model types and explanations for performance differences.


dataset can be access through kaggle; https://www.kaggle.com/datasets/abdkhan567/meme-dataset/settings
