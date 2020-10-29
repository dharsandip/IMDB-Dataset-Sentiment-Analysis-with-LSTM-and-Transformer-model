This project is based on IMDB movie review large dataset. This dataset has been downloaded from kaggle. 
Here, Sentiment Analysis (NLP) of the movie review data has been done using LSTM model (RNN)and also using a pre-trained Transformer model. 

Content of the dataset:
two columns (text : the review of the movie and label : the sentiment label of the movie review)


---------------------------------------------------------
Results:
---------------------------------------------------------

LSTM Model (RNN):

Accuracy of the Training set:  95%
Accuracy of the Test set:  85.74%

Classification report:

 precision    recall  f1-score   support

           0       0.89      0.81      0.85      4019
           1       0.83      0.90      0.86      3981

    accuracy                           0.86      8000
   macro avg       0.86      0.86      0.86      8000
weighted avg       0.86      0.86      0.86      8000


Model Summary:

Model: "sequential"
______________________________________________________________
Layer (type)                 Output Shape              Param #   
==============================================================
embedding (Embedding)        (None, None, 64)          7352832   
______________________________________________________________
lstm (LSTM)                  (None, 32)                12416     
______________________________________________________________
dense (Dense)                (None, 32)                1056      
______________________________________________________________
dropout (Dropout)            (None, 32)                0         
______________________________________________________________
dense_1 (Dense)              (None, 2)                 66        
==============================================================
Total params: 7,366,370
Trainable params: 7,366,370
Non-trainable params: 0

Pre-trained Transformer Model:

Accuracy of a Sample Test set:  73.11%

Classification report:

precision    recall  f1-score   support

           0       0.68      0.97      0.80       245
           1       0.92      0.45      0.60       205

    accuracy                           0.73       450
   macro avg       0.80      0.71      0.70       450
weighted avg       0.79      0.73      0.71       450






