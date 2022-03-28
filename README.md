# CS-301-Project
We will be investigating the task of predicting the genres of unlabeled music files. It is useful in cases where a song may need to be identified using only audio (like Shazam). It can also be further used for efficient music organization and music recommendation systems. This [paper](https://csitcp.com/paper/10/109csit05.pdf) published by Tecnológico de Monterrey, México, gives context and previous examples of music genre classification using basic classification algorithms and neural networks. We will use this paper as a reference and an example to help and guide our efforts. We will be using a precurated dataset from a [Kaggle Competition](https://www.kaggle.com/competitions/kaggle-pog-series-s01e02), consisting of 30 second clips of over 20,000 royalty free song samples in ogg format and their annotated musical genres to train the model. In order to analyze and classify each clip, we will have to obtain the shape, frequency, and other characteristics of each audio clip. We will use librosa to generate this data, and MatPlotLib to create visualizations of the data to help us qualitatively judge the effectiveness of our algorithm. Since this is a multiclass classification problem, we plan to use decision trees to start, and if necessary (and time permits), we will graduate to a neural network using TensorFlow. We will generate visualizations of the data in the form of spectrograms, and qualitatively assess the efficacy of the algorithm. We will also generate the error through the loss function of a decision tree, and upon the creation of our neural network algorithm, we will use the built in error function methods of TensorFlow to quantitatively evaluate our algorithms. We plan to plot the loss, and generate a figure/ bar graph of correctly identified audio clips versus the genre of the clip.
