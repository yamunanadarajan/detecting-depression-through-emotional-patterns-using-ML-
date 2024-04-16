# Detecting-depression-through-emotional-patterns-using-ML-
# Generate Sub-Emotions
Using an emolex lexicon to create the sub-emotion,EmoLex, or the NRC Word-Emotion Association Lexicon, is a list of English words and their associations with eight basic emotions and two sentiments. The emotions are: anger, anticipation, disgust, fear, joy, sadness, surprise, trust, The sentiments are negative and positive. Converting each word in the lexicon to a vector using Word2Vec. Then cluster the vectors using the AP clustering algorithm. Find the average value of each cluster, which represents the sub-emotions.
# Convert Text to Sub-Emotions
E-Risk 2018 data set was the DTA set used. which is a compilation of Redit users' posts. Tokenize and preprocess the text. Following preprocessing and tokenization, we have a set of terms for every user. Next, use Word2Vec to transform each word into a vector format. then figuring out how similar each word is to each of the sub-emotions, For every word, substitute the nearest sub-emotion. A sub-emotion is now assigned to every word.We then received a masked document for every user.
# BoSE Representation
Each masked document d is represented as a vector of weights associated to sub-emotion, the weight is computed in a tf-idf fasion.
# Classification
Feature selection using PCA (principle component analysis) and correlation analysis, classification done by SVM,and Dission tree classification methods.
