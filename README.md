# Unintended-Bias-in-Toxicity-Classification-Kaggle

Kaggle Unintended Bias in Toxicity Classification Challenge: https://www.kaggle.com/c/jigsaw-unintended-bias-in-toxicity-classification <br />
<br />
Current ensemble model ranks **377<sup>th</sup>** on Private LB with custom Bias AUC score of **0.93832** against Private LB highest of 0.94734 <br />
<br />
**Ensemble Details:**
1. BiLSTM model with 5-fold CV trained using FastText + GloVe embeddings (300d each)
2. BERT baseline fine-tuned over current dataset

**Potential Areas of Improvement:**
1. Finetune BERT baseline over entire training set (present limit is 50% due to computational constraints)
2. Try ensembling different BERT baselines (cased / uncased)
