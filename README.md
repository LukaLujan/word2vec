# Word2Vec project review

First - sometimes parts of the jupyter code won't render properly on the github, in that case just copy paste github code link into this online aplication; 
https://nbviewer.org/

And here is an example of the first part:
https://nbviewer.org/github/LukaLujan/word2vec/blob/main/gthb1.ipynb

In those 4 google colab notebooks we will test full usage of Word2Vec models.
About Word2Vec you can read more here; https://code.google.com/archive/p/word2vec/
We will use simple fake news data set. https://www.kaggle.com/c/fake-news/

We will try to predict what is fake news what is real news. Data is separated on the train.csv, test.csv and submit.csv(y label only)
Word models, in our example we will be using a model that has 3 million of the words and phrases , each with its own 300 dimension vector. 
Or you can use Word2Vec network, and train your own model, get your own vectors for each word in your corpus(compilation of the documents on which our model will be trained). 
After we train our model(or we use pre-trained model) , we need to preprocess data, do data embedding, and padding. Our keras deep learning network, that will try to predict "based on news article title - are those news fake or real"; need to be trained on numbers. All this preprocessing, embedding and padding will prepare our model to learn and do some real prediction.
Of course, after train our model on "train-validation" method, we will test it on test data, that our model haven't seen before. Test data is in separated csv format. That test data will also be "converted to numbers". 
We will do on 3 different ways. In the first notebook, we will create our own word embedding with word2vec network. In second colab network we will test our neural network on already pretrained word embeddings from large Word2vec vocab trained on billions of the words.
In third notebook, we will try to combine both pretrained model and our own model that will train on corpus. However because having two models working at the same time is a huge strain on google colab RAM(12gb limit). Because that, on first notebook(with number 3) we will do only preprocessing of both train and test data. We will learn how to save those numpy arrays, and how to load them in 4th notebook, where will use "fresh" RAM where we will create or model and see how far it will in this case.
