# STABLE-DIFFUSION
## About the project
### This project uses a Xception-based CNN to extract visual features from images and feed the information to a LSTM to generate corresponding captions. Xception is a pre-trained CNN model on the ImageNet database with python and Keras deep learning library. It has the highest accuracy compared to VCG16, VCG19, Resnet50, and Inception V3 with a rather small number of trainable parameters. Here, we use the pre-trained Xception model available in Keras and perform transfer learning on our image data to extract the visual features. Then we pass the captions of the training data through a LSTM, concatenate each learned textual feature after the visual features, and optimize the model using categorical entropy loss with adam optimizer.
## Dataset used
### Flickr_8K Dataset
### https://drive.google.com/file/d/1n7VwEPyrzCIPPAZNi0vn7pwPGJvR7hBA/view?usp=sharing
## Libraries Used
### string - Processing caption text
### OpenCV & NumPy - Reading and processing images
### pickle - used to store and load models/data
### Keras - High-level neural network framework on top of Tensorflow. We use it to build our own CNN+LSTM model on top of its pre-trained Xception model.


