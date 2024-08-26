 # Developing a deep learning model
 You can build a deep learning model using: 
- supervised learning
- unsupervised learning
- semi-supervised learning

Model development consists of
1. Data preparation
2. designing the model
3. training the model using training data
4. testing its performance 
5. deployment

### Data preparation 
  1. collect any form of data (text, images, videos, audio files, et cetera) from an external source
  2. convert the data to numeric values suitable for model training. These numeric values are in form of tensors.Then tensors need to be pre-processed during transforms,and we group them with batches that can be passed into the model.
  3. We take the data set and split it into three data sets: training data, validation data, and testing data.
### Training
  When we design the model, we use training data to train its parameters.
### Testing
  The next step is the testing step when we perform back propagation and validate the model by passing invalidation data, meaning we measure model's performance against unseen data and tune in hyperparameters.

  #### But what is the difference between training data and validation data?
  One of the common problems in deep learning is overfitting.Basically, model becomes really good at recognizing what it has been trained on,but cannot recognize examples it hasn't seen. In order to prevent that, we use the validation set.Validation is a crucial step in measuring your model's performance. During this process,you can evaluate training data against validation data that has never been used. 
  
  ### Deployment
  In the last step called model deployment, you can save the model to the file or deploy the model to a product or service. The model is usually deployed to a production environment on a cloud server or to an edge device. 