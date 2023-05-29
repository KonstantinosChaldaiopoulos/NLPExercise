# NLPExercise
An exercise for the NLP lesson in Artificial Intelligence MSc Program in Democritus.

## First part

The first part consists of the files En_core_web_sm.ipynb, NTLK_method.ipynb, bert_base_case_method.ipynb.This is the first part of an exercise that involves tokenizing a set of texts using three different methods and analyzing the resulting token frequencies.  The repository contains the completed code for tokenization using nltk.word_tokenize(), en_core_web_sm model from spaCy, and BertTokenizer from HuggingFace, as well as the analysis of token frequencies, including the number of tokens and unique tokens found, a randomly selected sentence and its token list, a table with the 20 most frequent tokens, and a log plot comparing the actual frequencies to Zipf's predictions with the best value of the constant A.

## Second part

The second part consists of the bigram and trigram models.

In the second part, we were asked to train and evaluate bigram and trigram language models on a collection of 199 news articles from the Wall Street Journal, using the first 170 articles for training and the remaining 29 for evaluation. Specifically, we trained four models with bigram and trigram sizes for uppercase and lowercase letters and smoothing parameters of k=1 and k=0.01, and evaluated their performance using the perplexity metric.

During the training phase, we replaced all tokens that appear in the training set less than three times with an "UNK" token, and added all remaining tokens to the model's vocabulary. We also added special tokens to mark the beginning and end of each sentence, respectively.

We then evaluated the models on the evaluation set, computing their perplexity both on the original text and on a lowercased version of the text. We also generated three new sentences using each model, sampling words based on their probability according to the model.

Overall, this exercise provided a hands-on experience with training and evaluating language models, and allowed us to explore the impact of n-gram size, smoothing, and lowercasing on their performance.

## Authors
This repository was created by Konstantinos Chaldaiopoulos
