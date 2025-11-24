# FurtherLearn-the-tutorial-Bag-of-Words-Meets-Bags-of-Popcorn
DeepLearningMovies
==================

本次任务不再使用Word2Vec进行。而是以GloVe进行

教程地址：https://www.kaggle.com/competitions/word2vec-nlp-tutorial

资料：

GloVe模型：https://github.com/stanfordnlp/GloVe

glove.840B.300d转为.gensim文件：https://github.com/manasRK/glove-gensim

### 目标：

1.数据清洗并创建GloVe特征

2.尝试早期的cnn、rnn、lstm和注意力机制训练并预测

3.生成预测结果

4.提交测评并统计得分

### 实验过程记录

1.得到glove.840B.300d文件后还不能于imdb_process.py中生成特征，需要转换为.gensim文件，
用“资料”中获取的glove-gensim.py生成glove.840B.300d.gensim文件。

2.glove.840B.300d.gensim文件置于目录下，运行imdb_process.py得到./pickle/imdb_glove.pickle3文件。

3.kaggle平台中导入model、testData.tsv。调整imdb_cnn等文件代码训练并预测得到对应结果。

4.生成的.csv文件包含25,000行加上一行头部，有两列：“id”和“sentiment”。提交到教程测评得到评分。

### 实验测评结果：

|        | cnn       | lstm       | cnnlstm      | attention_lstm       | gru      |
| :---------- | :---------- | :---------- | :---------- | :---------- | :---------- |
| 1st_test_Score     | 0.80728     | 0.50000     | 0.76300     | 0.87372     | 0.83928     |
| 2nd_test_Score     | 0.81132     | 0.78532     | 0.82540     | 0.84144     | 0.85720     |
