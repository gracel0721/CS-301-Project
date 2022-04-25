# Predicting Music Genres using Data Algorithms and Neural Networks
## Mohamed Akash, Grace Leverett, Amritha Venigalla

### Abstract
Traditional music style classification methods use many acoustic characteristics to label music with specific genres and styles. The design of characteristics necessitates musical knowledge and the characteristics of different classification tasks are not always consistent. The rapid development of neural networks and big data technology has provided a new way to better solve the problem of music-style classification, and it is important that we explore it in depth to have more efficient classification methods. We set out to develop a basic one using a Convoluted Neural Network.  
### Introduction
We were tasked with creating a machine learning algorithm to classify and predict the music genre of unlabeled audio clips. In this day and age, with the massive amount of music coming out and music data currently available, music style and genres are key ways to classify the music. They are the primary modes used to group music together and search for specific types of music. They take into account different features such as rhythm, melody and harmony. And with the vast amount of music data, it is no longer feasible to manually classify all the music that exists. With the rapid development of neural networks it is important to explore this to see how it can assist in automated music classification. 

### Related Work
  We reviewed a similar paper published by Tecnológico de Monterrey, México titled, [__Data-Driven Techniques for Music Genre Recognition__](https://csitcp.com/paper/10/109csit05.pdf). Their approach considered multiple different algorithms and tested them against each other. The algorithms used included a Fully Convolutional Neural Network (FCN), Random Forest (RF), and Linear Regression. Multiple implementations of each algorithm were used, with  both random forest algorithms ranking highest in both train and test accuracy. Additionally, we looked at some of the Kaggle submissions for the competition to see if there was anything that we considered that did not work, or worked really well. We decided to utilize a Neural Network to compare the bpm of each audio file, and the Mel-Frequency Cepstral Coefficient (MFCC). There were multiple kaggle entries that utilized this coefficient in some way, so we decided to implement it into our work. The methods utilized in the first paper proved slightly beyond our machine capabilities, as the compilation of our model took disproportionaltely long, even with the use of a GPU. As such we decided to use a CNN.
  
  ### Data
  Our dataset consists of short audio clips in the .ogg format. The data comes from a Kaggle Competition data set. There are about 20000 training files, and 5000 test files. Some of the files we wer given were corrupted, so those we could not restore, we discarded. This left approximately 19200 training files and 4850 test files. Unfortunately, since we were dealing with such a great deal of data, we were unable to complie the model using every file, as the compilation would take >10hours, and our runtime would disconnect before that mark. In total, we were able to use ~ 5600 training files and ~1000 test files.
  
  
  ### Methods
  In order to classify our model, we used a CNN comparing beats per minute of each clip. since so many genres have similar bpm, due to the emotion each gnere generally conveys (Pop tends to be happier, so it has a higher bpm, Blues tends to be sadder, so it has a lower bpm). Again, we did consider other methods and algorithms, such as an RF, or LIN but were limited by our machine capabilities with the amount of data we processed. 
  
  ### Experiments
  We considered a model with 3 hidden ReLU layers with 4, 3, and 2 neurons respectively, and a binary crossentropy loss model. We found this had a 64.3% loss rate, and a 54.2% accuaracy. We were able to conculde that this model was ineffective, which is very ineffective compared to the RF algorithms performed by Tecnológico de Monterrey. 
  
 
  ### Conclusion
  We cannot conclude that our model was effective, and we would like to further train and conduct experiments on this dataset, prefereably with a more powerful machine so all given data can be used. Given a better machine and more time, we would also like to compare our tested model to a Random Forest, as it has a much higher accuracy rate than our model.
