# MLEnd_hums_whistles_classification

MLEnd Hums and Whistles dataset (Requena, Bajaj and Sciola, 2022):
https://www.kaggle.com/datasets/jesusrequena/mlend-hums-and-whistles/discussion/326320

This repository consists of two jupyter notebooks solving two different classification problems using the MLEND hums and whistles dataset.

## Song Prediction
song_prediction.ipynb attempts to classify hum or whistle audio files as the Harry Potter Theme or the Imperial March. Using the librosa library, the tempo of each audio file is extracted as a lone feature. SVM, Naive Bayes or KNN are applied to the tempo feature, achieving 78.8% accuracy at binary classification.

## Key Prediction
key_prediction.ipynb attempts to predict the key (major or minor) of hums and whistles. Minor songs were the Harry Potter Theme, Imperial March and Pink Panther. Major songs were Hakuna Matata, Mamma Mia and Singing in the Rain. The basic approach was to generate frequency band data for each song interpretation and assume that the most hummed/whilsted note was the tonic of the key. By comparing the prevalence of major and minor thirds in the audio file, song key was predicted at 57.4% accuracy. Although final accuracy was low, the approach taken was novel and interesting to develop.
