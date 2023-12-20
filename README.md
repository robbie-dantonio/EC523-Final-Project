# EC523-Final-Project
Final project for BU ENG EC523: Deep Learning

## .ipynb notebooks 
We have four .ipynb notebooks in the repository, and one additional in the Best Model Single Character folder. Three of these notebooks are mostly the same, and have been used for testing different model architectures. All three have been trained at some point with varying architectures and parameters:
* Copy of Project.ipynb
* ProjectLSTM.ipynb
* ready_LSTM.ipynb

We also have a fourth notebook LSTM_Implementation.ipynb, in which we have implemented a LSTM block ourselves (instead of nn.LSTMCell).

## Error_Results Folder
This folder holds three .txt files, which contain loss data for three implementations:

* Loss_report.txt: CNN output 256
    - did not use batch normalization
    - included positional embedding.
    - changed the input size to 64*256
    - 16 number of batches
    - learning_rate = 0.0003 

* Loss_report2.txt: CNN output 512
    - Used batch normalization
    - included positional embedding
    - changed the input size to 32*1024
    - 64 number of batches
    - learning_rate = 0.0001

* Loss_report4.txt: CNN output 256
    - did not use batch normalization
    - did not use positional embedding.
    - changed the input size to 64*256
    - 64 number of batches
    - learning_rate = 0.0001 

## Best Model Single Character Folder
Contains the .ipynb and a .pt parameters folder for our model trained on different data containing images of individual LaTeX symbols. This data is generated from a function inside the .ipynb notebook. 
