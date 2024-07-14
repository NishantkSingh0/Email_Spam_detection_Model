# Email Spam Classification:
## Purpose of the Model
This model is prepared for the classification of emails as spam or not spam. The aim is to leverage transformer-based models to achieve high accuracy in detecting spam emails.

## Subclassing Method
The model is built using the subclassing method in TensorFlow, providing flexibility for modifications and improvements. This approach allows for custom layers and architectures, making the model adaptable to different tasks and datasets.

![Screenshot (100)](https://github.com/user-attachments/assets/6d9522ad-4c98-4029-8f86-51fecd57f102)

## Datasets:
Used HuggingFace "Deysi/spam-detection-dataset" dataset for Fine tuninng Bert 
![Screenshot (105)](https://github.com/user-attachments/assets/f5a5974e-fe9d-46f9-a23c-ff1fae01c712)

## Dataset Sample:
Hello,
I am taking a graduate level course on applied machine learning. The goal of the course is not to have a rigorous understanding of the mathematics behind ML algorithms, but to develop an intuitive sense for how to handle data and use it for an end-to-end ML project.\n\nTo this end, we are required to do a class project with a fairly rich (a good amount of features which I can later engineer) and large dataset. Pretty much the only requirement for the dataset is that it needs to have at least 1000 instance. While that seems like a small number, my professor has insisted that something like 1000 entries from time series data will not cut it. Instead, it has to be at least 1000 uniquely identifiable instances.\n\nMy background is in materials science and nanotechnology, but I cannot find any interesting datasets for the same which meets the above requirement.

### Label 'not_spam'

## Preprocessing of Datasets:
The preprocessing of the dataset involves the following steps:

Tokenization: The raw email text is tokenized using a pre-trained BERT tokenizer, which converts the text into tokens that the model can understand.
Padding and Truncation: The tokenized sequences are padded or truncated to ensure they have the same length, which is necessary for batch processing.
![Screenshot (101)](https://github.com/user-attachments/assets/f37f5ebe-a002-4bd9-b922-eef23a4dba21)

Encoding Labels: The labels (spam or not spam) are encoded into binary format, where 0 represents 'not spam' and 1 represents 'spam'.
![Screenshot (102)](https://github.com/user-attachments/assets/00365e0a-dd76-42d5-9ff1-99db0c21e2bc)

## Accuracy:
The model achieved a remarkable accuracy of 99.99% on both the training dataset and the test dataset, demonstrating its efficacy in classifying emails as spam or not spam.
![Screenshot (103)](https://github.com/user-attachments/assets/3f3cf27d-2b2f-469b-a354-3f275caeb175)
