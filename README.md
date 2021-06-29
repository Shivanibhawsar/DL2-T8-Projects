# DL2-T8-Projects
# **English-to-Hindi-Translator**
The model translates English text to Hindi text. The project was implemented in Keras Framework on TensorFlow. 
An encoder was used to convert the English phrases to feature vectors that can be trained upon and a decoder converts the output vector back to normal Hindi text (utf-8).

## DATASET
The dataset consist of 127607 rows and 3 columns of English phrases along with their Hindi translations. The data is given in utf-8 format.

## Data Cleaning
- removing missing values
- removing duplicate rows
- lowercase all letters
- remove quotes
- remove all special characters
- remove all numbers from text
- remove extra spaces

## **MODEL**
### _Encoder_
Encoder takes the English data as input and converts it into vectors that is passed to an LSTM model for training. We discard the encoder output and only keep the states.

### _Decoder_
The decoder takes in Input the states of the encoder and the Hindi data points corresponding to the English input of Encoder. It trains an LSTM to produce the translated phrase in output. The decoder used softmax layer.

## TRAINING
The model was trained using LSTM on My PC. So no use of GPU. The model was trained in parts due to lack of computational power. It was run for 100 epochs at a time which took around 1 hr for only 10 epochs . Used categorical_crossentropy loss. Used rmsprop optimizer. The data was passed to the model in batches of size 128. 

## MODULES

- ANACONDA  -  https://www.digitalocean.com/community/tutorials/how-to-install-anaconda-on-ubuntu-18-04-quickstart
- Jupyter Notebook - https://jupyter.readthedocs.io/en/latest/install.html
