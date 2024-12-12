# Image Classification Task  

## Dataset Details  
A dataset of ~ 25K images (each of size 150 x 150) is used.  
Each image has a label from the following 6 categories:  
{'buildings': 0, 'forest': 1, 'glacier': 2, 'mountain': 3, 'sea': 4, 'street': 5}.  

The images are divided into 3 subsets:  
- TRAIN (folder: seg_train): ~14K  
- VALIDATION (folder: seg_test): 3K  
- PREDICTION (folder: seg_pred): 7K  

## Tasks  

### 1. Fully-Connected Feed-Forward Neural Network  
- Use a fully-connected feed-forward neural network with H hidden layers (each containing N neurons) to classify the dataset.  
- Use some fixed values of H and N, e.g., H = 2, N = 100.  
- Use the validation set to determine the number of epochs for early stopping.  
- Apply dropout and other regularization techniques.  

### 2. Convolutional Neural Network (CNN)  
- Use a Convolutional Neural Network to perform the same task as described in (1).  
- Example architecture:  
  (CONV - ReLU) -> MAXPOOL -> (CONV - ReLU) -> MAXPOOL -> (FC - ReLU) -> (FC - SOFTMAX).  
- Apply dropout and other regularization techniques.  
