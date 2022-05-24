# Abstractive Text Summarization of News Using Pre-Trained Transformers

##

## Motivation:

With a more global society today than ever, staying informed on current events is a time-consuming task. Fortunately, with advances in Natural Language Processing, tools have developed that can analyze text-based data and perform various classification and generative tasks. 

These tasks has traditionally been very hard to tackle as language can be ambiguous, abstract, but is also highly context dependent in complex ways as there may exists both short and long-term contextual information.

##

## How:
In this project the goal is to fine-tune two pre-trained networks from the HuggingFace API using news articles. These networks will then be used to generate a summary of news article, that can be compared to a highlight of the article which is written by the articles author. The two networks that are utilized for the abstractive text summarization is the T5-Small and BART. 

##

## Data: 
The data set used in this project is the CNN/Daily Mail summarization dataset. It consists of 311 971 unique news articles that is written by journalists at CNN, and the Daily Mail. The data set is split into 287 113 articles in the training set, 13 368 in the validation set and 11 490 in the test set. Each observation in the data set consists of three columns: an ID, the news article, and a highlight written by the articles author which summarizes the main points of the article.



## Results: 

An excerpt of the results for both models are shown, only displaying the Precision, Recall and F-measure for the Rouge-Lsum metric. 

### T5-Small:

| Rouge-1 | Low | Mid | High |
| --- | ---:| ---: | ---: |
| Precision |0.40 | 0.41 | 0.41 |
| Recall | 0.27 | 0.27 |  0.28 |
| F-measure   |  0.32 | 0.32 |  0.32 |  



### BART:

| Rouge-1 | Low | Mid | High |
| --- | ---:| ---: | ---: |
| Precision | 0.38 | 0.38  | 0.39 |
| Recall | 0.39 | 0.39  | 0.40 |
| F-measure   | 0.38  | 0.38  | 0.38 |   
