### Project: Classify Consumer  Complaints

### Highlights:

 - This is a **multi-class text classification (sentence classification)** problem.
 - The purpose of this project is to **classify Kaggle Consumer Finance Complaints into 11 classes**. 
 - The model was built with **Convolutional Neural Network (CNN)** and **Word Embeddings** on **Tensorflow**.

### Data: [Consumer Complaints]

 - Input: **consumer_complaint_narrative**

    
 - Output: **product**


### Train:

 - Command: python3 train.py training_data.file parameters.json
 - Example: ```python3 train.py ./data/consumer_complaints.csv.zip ./parameters.json```
 
 A directory will be created during training, and the best model will be saved in this directory. 

### Predict:

 Provide the model directory (created when running ```train.py```) and new data to ```predict.py```.
 - Command: python3 predict.py ./trained_model_directory/ new_data.file
 - Example: ```python3 predict.py ./trained_model_1479757124/ ./data/small_samples.json 2> Prediction.txt;```

### Reference:
 - [Implement a cnn for text classification in tensorflow](http://www.wildml.com/2015/12/implementing-a-cnn-for-text-classification-in-tensorflow/)
