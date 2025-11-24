# FurtherLearn-the-tutorial-Bag-of-Words-Meets-Bags-of-Popcorn
DeepLearningMovies
==================

本次任务不再使用Word2Vec进行。而是以GloVe进行

教程地址：https://www.kaggle.com/competitions/word2vec-nlp-tutorial

资料：

GloVe模型：https://github.com/stanfordnlp/GloVe

glove.840B.300d转为.gensim文件：https://github.com/manasRK/glove-gensim

# 目标：

1.数据清洗并创建GloVe特征

2.尝试早期的cnn、rnn、lstm和注意力机制训练并预测

3.生成预测结果

4.提交测评并统计得分


# 实验测评结果：

|        | cnn       | lstm       | cnnlstm      | attention_lstm       | gru      |
| :---------- | :---------- | :---------- | :---------- | :---------- | :---------- |
| No.1_test     | 0.80728     | 0.50000     | 0.76300     | 0.87372     | 0.83928     |
| No.2_test     | 0.81132     | 0.78532     | 0.82540     | 0.84144     | 0.85720     |
