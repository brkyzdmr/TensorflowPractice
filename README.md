# Tensorflow Applications
These applications are based on the information learnt in the [TensorFlow in Practice Specialization](https://www.coursera.org/specializations/tensorflow-in-practice). 


## Table of contents

- [Tensorflow Applications](#Tensorflow-Applications)
  - [Table of contents](#Table-of-contents)
  - [Prerequisites](#Prerequisites)
  - [Possible Issues](#Possible-Issues)
  - [Convolutional Neural Networks](#Convolutional-Neural-Networks)
    - [Basic Applications](#Basic-Applications)
    - [Advanced Applications](#Advanced-Applications)
  - [Natural Language Processing](#Natural-Language-Processing)
    - [Basic Applications](#Basic-Applications-1)
    - [Advanced Applications](#Advanced-Applications-1)
      - [IMDB Reviews Classification Comparison (Subwords)](#IMDB-Reviews-Classification-Comparison-Subwords)
      - [IMDB Reviews Classification Comparison](#IMDB-Reviews-Classification-Comparison)
      - [News Headline Sarcasm Classification Comparison](#News-Headline-Sarcasm-Classification-Comparison)
  - [Sequences, Time Series and Prediction](#Sequences-Time-Series-and-Prediction)
    - [Basic Applications](#Basic-Applications-2)
    - [Advanced Aplications](#Advanced-Aplications)


## Prerequisites
- Some of the applications are using `Tensorflow 2.0.0-rc1` and mostly others are using `Tensorflow 1.14.0`. You can create seperate conda environment for both version. I recommend gpu versions for fast training.

```shell
pip install tensorflow-gpu==1.14.0
```

```shell
pip install tensorflow-gpu==2.0.0-rc1
```

- Before you train in gpu you have to install and configure CuDNN, Cuda and Nvidia driver. For more information [Tensorflow2.0.0 GPU Support](https://www.tensorflow.org/install/gpu)

- Most of the application using specific dataset. Thanks to `wget` command, you don't need to effor for downloading them, just run the predetermined cell. 

## Possible Issues
- If you can't plotting the result just re-run the cell.
  ```shell
  <Figure size 640x480 with 1 Axes>
  <Figure size 640x480 with 1 Axes>
  ```
- If you install all of the gpu prerequisites, but still getting error:
  ```shell
    nvidia-smi
  ```
  Look-up the nvidia gpu memory usage, kill all of the process with `kill [process-pid]`.

- If you worrying about some of the applications training time, don't worry if one epoch took less than 15 min. (Especcially for NLP applications)

## Convolutional Neural Networks
### Basic Applications
- [Housing Price Prediction with Single Perceptron](/Applications/Housing_Price_Prediction_with_Single_Perceptron.ipynb)
- [Fashion Recognition Using Deep Neural Network](/Applications/Fashion_Recognition_(DNN_and_CNN).ipynb)
- [Handwritten Digit Recognition](/Applications/Handwritten_Digit_Recognition.ipynb)
- [Horse-Human Classifier Using CNN](/Applications/Horse-Human_Classifier_Using_CNN.ipynb)
- [Cat-Dog Classifier Using CNN (3k Images)](/Applications/Cat-Dog_Classifier_(3k_Images).ipynb)
- [Cat-Dog Classifier Using CNN (25k Images)](/Applications/Cat-Dog_Classifier_(25k_Images).ipynb)
- [GPU Training Test](/Applications/GPU_Training_Test.ipynb)
- [Multi Categorical Classification](Applications/Multi_Categorical_Classification.ipynb)
- 
### Advanced Applications
-  [Image Augmentation](/Applications/Image_Augmentation.ipynb)
-  [Transfer Learning and Drop-out](/Applications/Transfer_Learning_and_Drop-out.ipynb)
- [Hand Gesture Recognition](/Applications/Hand_Gesture_Recognition_Using_CNN.ipynb)

## Natural Language Processing
### Basic Applications
- [Sentiment in Text](\Applications/Sentiment_in_Texts.ipynb)
- [Sentiment Preprocessing in BBC Text Archive](\Applications/Sentiment_Preprocessing_in_BBC_Text_Archive.ipynb)
- [Sentiment Preprocessing in Sarcasm Detection Dataset](\Applications/Sentiment_Preprocessing_in_Sarcasm_Detection_Dataset.ipynb)
- [Text Classification Using Word Embeddings In IMDB Reviews Dataset](/Applications/Text_Classification_Using_Word_Embeddings_In_IMDB_Reviews_Dataset.ipynb)
- [Text Classification Using Word Embeddings In BBC News Archive](/Applications/Text_Classification_Using_Word_Embeddings_In_BBC_News_Archive.ipynb)
- [Text Classification Using Word Embeddings In IMDB Reviews Dataset (Subwords8k)](/Applications/Text_Classification_Using_Word_Embeddings_In_IMDB_Reviews_Dataset(Subwords8k).ipynb)

### Advanced Applications
- [Exploring Overfitting in NLP](/Applications/Exploring_Overfitting_in_NLP.ipynb)
- [Creating Shakespeare Sonnets Using LSTM](/Applications/Creating_Shakespeare_Sonnets_Using_LSTM.ipynb)

#### IMDB Reviews Classification Comparison (Subwords)
- [IMDB Subwords 8K with 1D Convolutional Layer](/Applications/IMDB_Subwords_8K_with_1D_Convolutional_Layer.ipynb)
- [IMDB Subwords 8K with Single Layer LSTM](/Applications/IMDB_Subwords_8K_with_Single_Layer_LSTM.ipynb)
- [IMDB Subwords 8K with Multi Layer LSTM](/Applications/IMDB_Subwords_8K_with_Multi_Layer_LSTM.ipynb)

#### IMDB Reviews Classification Comparison 
- [IMDB Reviews Classification with 1D Convolutional Layer](/Applications/IMDB_Reviews_Classification_with_1D_Convolutional_Layer.ipynb)
- [IMDB Reviews Classification with Bidirectional GRU](/Applications/IMDB_Reviews_Classification_with_Bidirectional_GRU.ipynb)
- [IMDB Reviews Classification with Bidirectional LSTM](/Applications/IMDB_Reviews_Classification_with_Bidirectional_LSDM.ipynb)

#### News Headline Sarcasm Classification Comparison
- [Sarcasm Classification with 1D Convolutional Layer](/Applications/Sarcasm_Classification_with_1D_Convolutional_Layer.ipynb)
- [Sarcasm Classification with Bidirectional LSTM](/Applications/Sarcasm_Classification_with_Bidirectional_LSTM.ipynb)

## Sequences, Time Series and Prediction
### Basic Applications
- [Creating Random Time Series](/Applications/Creating_Random_Time_Series.ipynb)
- [Creating Dataset](/Applications/Creating_Dataset.ipynb)
- [Naive Forecasting in Time Series](/Applications/Naive_Forecasting_in_Time_Series.ipynb)
- [Time Series Prediction with Single Layer Neural Network](/Applications/Time_Series_Prediction_with_Single_Layer_Neural_Network.ipynb)
- [Time Series Prediction with DNN](/Applications/Time_Series_Prediction_with_DNN.ipynb)

### Advanced Aplications
- [Time Series Prediction with RNN](/Applications/Time_Series_Prediction_with_RNN.ipynb)
- [Time Series Prediction with LSTM](/Applications/Time_Series_Prediction_with_LSTM.ipynb)
- [Time Series Prediction with CNN and LSTM](/Applications/Time_Series_Prediction_with_CNN_and_LSTM.ipynb)
- [Sunspot Prediction with CNN and LSTM](/Applications/Sunspot_Prediction_with_CNN_and_LSTM.ipynb)