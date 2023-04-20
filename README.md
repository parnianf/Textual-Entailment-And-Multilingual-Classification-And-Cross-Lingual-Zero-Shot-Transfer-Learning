# Textual-Entailment-And-Multilingual-Classification-And-Cross-Lingual-Zero-Shot-Transfer-Learning



## Part 1: [ParsiNLU](https://arxiv.org/abs/2012.06154) dataset Classification (Textual Entailment)
In this question, we intend to use Transformers in text application. One of the applications in the Natural Language Processing studied is Textual entailment. Textual entailment is a classification that can be used to understand the relationship between two sentences. In this assignment there are 3 relationships:

1. **Entailment**: In this case, the first sentence proves that the second sentence is correct.
2. **Contradiction**: There is contradiction between the two sentences.
3. **Neutral**: The sentences are not related to each other.

In this task we are to use contextualized word embedding like `BERT`.

The main topics discussed in this part are:
* The need of preprocessing data
* Implementing a neural network to classify the data using `XLM-RoBERTa`. This model is available in [Hugging Face](https://huggingface.co/xlm-roberta-base).
* Implementing a neural network to classify the data using `ParsBERT`


#### Dataset
One of the datasets published by the ParsiNLU article is related to the Textual Entailment task. This dataset is available here:
https://huggingface.co/datasets/persiannlp/parsinlu_entailment

## Part 2: Multi-lingual & Mono-lingual classification

The main topics discussed in this part are:
* Implementing a neural network to classify the English data using `BERT`.
* Implementing a neural network to classify the Persian data using `ParsBERT`.
* Implementing a neural network to classify the Persian & English data together using `XLM-RoBERTa`.


#### Dataset
The dataset is in *Question2_Data* folder given. This dataset has three columns: **source** (English text), **targets** (translated Persian text) and **category** (including three tags: **Quran**, **Bible**, **Mizan** (collection of literary masterpieces translated into English)).


## Part 3: Cross-lingual zero-shot transfer learning

According to [this paper](https://arxiv.org/abs/2101.10649), in zero-shot cross-lingual transfer, a supervised NLP task trained on a corpus in one language is directly applicable to another language without any additional training.

According to [this paper](https://aclanthology.org/P19-1299.pdf), some NLP tasks are not applicable to most human languages due to the lack of annotated training data for various NLP tasks. Cross-lingual transfer learning (CLTL) is a viable method for building NLP models for a low-resource target language by leveraging labeled data from other (source) languages which have more labeled data.

I can mention that sometimes it is better to have a large labeled data in another language than training the model with small data with the same language as test data.

In this part, I train the model on English data and test it on Persian data.

#### Dataset
The dataset is in *Question2_Data* folder given. This dataset has three columns: **source** (English text), **targets** (translated Persian text) and **category** (including three tags: **Quran**, **Bible**, **Mizan** (collection of literary masterpieces translated into English)).

## Report
Report is available [here](https://github.com/parnianf/Textual-Entailment-And-Multilingual-Classification-And-Cross-Lingual-Zero-Shot-Transfer-Learning/blob/main/NLP_CA4_Report_English.pdf).
