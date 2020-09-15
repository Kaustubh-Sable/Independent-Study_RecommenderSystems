In this project, I have used word2Vec for recommending the songs to the user.

#### Background
Word2vec are neural network models that were initially introduced for learning word embeddings that are highly useful for Natural Language Processing tasks.
I have used Skip-gram word2vec model for the project which can be defined as a shallow neural network with a single hidden layer that takes in a word as input and tries to predict the context of words around it as output (in terms of NLP).

#### Introduction

So, you wonder what will neural network look like with songs instead of words? Here it is how:
![Word2Vec For Songs](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Playlist_Generation/Images/word2VecForSongs.png)

Using Word2vec, we have transformed our problem of finding songs that appear in similar contexts into mathematical numbers that capture those local co-occurrences. We can look at the weights as coordinates in a high dimensional space, with each song being represented by a point in that space. 

Here is how we visualize this space usign t-SNE where each point in the space represent a song:
![Song Vector Space](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Playlist_Generation/Images/SongVectorSpace.png)

Here is great animation how song vectors help to recommend song to a particular user: https://cdn-images-1.medium.com/max/1400/1*xbNM_CnEIWQtGbsLmZtE-A.gif

##### Dataset

The spotify dataset used in the program can be downloaded from http://dbis-nowplaying.uibk.ac.at/ 

### Procedure
The code includes the following phases:
1. Preprocessing and feature engineering
2. Training the Word2Vec Music Recommender
3. Evaluation (using NDCG)
4. Example recommendations
5. Visualizing embeddings

### Results
This is a sample result where a playlist is generated based on the given song as seed:

![Playlist Generation](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Playlist_Generation/Images/examplerec.png)

#### Notes
* More information on NDCG and word2Vec can be found in this [presentation](https://github.com/Kaustubh-Sable/Independent-Study_RecommenderSystems/blob/master/Slides/KS_Week8_Reco_Sys.pptx).
* The python notebook can also be seen live on Google Colab here: https://colab.research.google.com/drive/1JfBOezfVWyYre219HND-0PmDlNvJJshS?usp=sharing

#### References
* Related research Paper: https://arxiv.org/pdf/1804.04212.pdf 
* Related Blog: https://towardsdatascience.com/using-word2vec-for-music-recommendations-bb9649ac2484 

