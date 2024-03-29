# Recycle Me ML Development

Repository of Machine Learning Development for Bangkit Capstone Project CH2-PS491 Team Recycle Me App

## Notebooks

### waste_classification_transfer

- Notebook for training the waste classification model
- Model trained using transfer learning from MobileNetV3Small pretrained model

### sentence_encoder_USE_clean

- Notebook for generating the embedding of recycling article titles from the English translation of the titles
- The embeddings is generated using the Universal Sentence Encoder, which is a model for generating embeddings from English sentences

### recycling_article_title_encoder_model

- Notebook for training the sentence encoder model that takes recycling article titles in Indonesia, generates the embedding, and computes the similarity of each title with the others
- The training uses inputs consisting of article titles in Indonesian, and the labels are the results of embedding from the translation of these titles into English, which was generated earlier using the sentence_encoder_USE_clean notebook.
- The trained model can generate embeddings of recycling article titles in Indonesia that are similar to the embeddings produced by the Universal Sentence Encoder from their English translation

## Folder

### dataset

Contains datasets used for training the model. This folder also contains the recycling article dataset with computed similar titles.

### model

Contain the waste classification model in tflite format

## Module Requirements

- numpy
- pandas
- matplotlib
- tensorflow
- tensorflow_hub
- keras
- sklearn
- zipfile
- pathlib
- os
- csv
