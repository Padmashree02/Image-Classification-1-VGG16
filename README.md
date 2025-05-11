# Problem - Image classification with Deep neural network

Transfer learning and Fine-tuning a pretrained model is the method to train the model as per the desired output.

> Example- if the model has to classify the new class or optimize the model with more accuracy values.

There are techniques involved in fine-tuning the model, such as either the pre-existing layers can be freezed and change the last layer, or tweak the already trained layers as per our need.

> My solution of fine-tuning is by changing last layers with my custom layers. While training, the model's trained layers are freezed to maintain their weights and prevent from overfitting which can loose the cardinal informations from the image. Thus, the model will be trained with addition of new layers.

Solution :-

  > Network/Layer - VGG16

  > Framework - Tensorflow (Tensorflow.Keras)

  > Dataset (while training the network) - Customized dataset

  > Library - cv2, numpy, matplotlib.pyplot

  > Topic - VGG16, layers, optimizers, fine-tuning, data generator

  > Pipeline :-
 
      : import the model from tensorflow.

      : Load the customized dataset

      : Preprocess the dataset as per the VGG16's network configuration.

      : Intialize the VGG16 network with its own weights.

      : Freeze all the VGG16's pre-existing layers.

      : Define the custom layers.

      : Perform image generator to each pre-processed dataset (train and valid).

      : Configure the model.

      : Train VGG16 with new layers with new dataset.

      : Save the trained model (optional)

      : Evaluate the trained model to anlayse how well the model has been trained in training phase.
      
      : Test the trained model with new images, to test how well the model reacts with new images. 
