
# A study of Emotion Detection on COVID-19 related Misinformation on Twitter

MSc Dissertation: Artificial Intelligence

School of Electronic Engineering and Computer Science -
Queen Mary University London, United Kingdom

Supervisor: Matthew Purver

## Abstract

Increase in social media usage during the COVID-19 pandemic has also given rise to misin- formation and fake news. Misinformation and fake news cause powerful emotional reactions in the public, which can potentially aid their propagation. Analysing the emotional state of the public towards fake news can help us gain insight about the rapid spread of misinformation and ways to combat it. Emotions are complex and emotion detection remains a difficult task. This paper explores models for multi-label emotion classification which utilise the BERT archi- tecture as well as emotion lexicon information to accurately analyse the emotional responses of the public to known COVID-19 misinformation tweets. Experiments on the SemEval 2018, Task 1 dataset demonstrate the model’s strength, achieving a state of the art result on sub- task E-c for English tweets. Using the model, we find that misinformation provokes significant emotional responses from people on Twitter, especially negative emotions like anger and disgust, and it also creates mistrust towards potentially influential accounts such as government officials.

## Structure

The following is a description of each notebook in the project.

**SemEval.ipynb** - Trains and tests our model with the best performing parameters on the SemEval dataset.

**Lexicon.ipynb** - Trains and tests the lexicon based approach to SemEval.

**Plutchik.ipynb** - Trains the version of the model that will be used for inference using SemEval+COVIDEmo datasets.

**TweetRetrieval.ipynb** - This is a notebook for retrieving text from tweet IDs for COVIDEmo and Misinformation tweets.

**ReplyRetrieval.ipynb** - This is a notebook for retrieving the reply text for wanted IDs. A dataset of such retrieved IDs has been made public [here](https://github.com/dimitrismylo/Misinformation-Reply-Dataset).

**Misinformation.ipynb** - This is a notebook for conducting inference and analysis on the reply dataset.

## Model and Lexicons

The final trained model has been made available on HuggingFace [here](https://huggingface.co/dimitrismylo/SemEval_BERTweet/tree/main).

Lexicons used in this project:

* [NRC Emotion](https://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm)
* [NRC Hashtag Emotion](https://saifmohammad.com/WebPages/lexicons.html)
* [Multidimensional Lexicon of Emojis](https://www.rebeccagodard.com/multidimensional-lexicon-of-emojis-mle)