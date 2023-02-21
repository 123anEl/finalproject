# finalproject



FINAL PROJECT REPORT
on the topic of:
"Dog breed classification"




Student:
 Anel Onlan
 
Instructor: 
Sultanmurat Yeleu


Astana, 2023











Introduction 

Problem 

Lost pets are one of the main causes of stray animals. The dogs we see on the street are either discarded, or lost, or offspring from both. They pose a great threat to people, as they can attack them. According to informburo.kz in April-May 2022, 50 bites and scratches were recorded in Aktobe, 30 of which were pet aggression. For this reason, in order to reduce the occurrence of stray dogs, it is possible to help return lost dogs to their owners. To do this, it is achievable to create a program that will search through the cameras for a particular breed of dog, which will significantly reduce the time for searching.

Literature review with links (another solutions) 

https://www.linkedin.com/pulse/did-you-know-app-detects-lost-pets-through-artificial-imran-alam/

https://blog.xmartlabs.com/blog/deep-learning-approach-for-dog-identification/

https://www.news9live.com/technology/forpaws-will-use-facial-recognition-and-machine-learning-to-help-find-your-lost-pet-133977

Current work (description of the work) 

At the moment the model takes only the first 20 categories of dogs. Since, the dataset is excessively large. Then, the model resizes images to 227 x 227 because the input image resolution for AlexNet is 227 x 227. Next, the model prints 9 different images and predicts almost the same breed as in the original picture.

Data and Methods

Information about the data  

Data was taken from Kaggle datasets. This dataset contains 20,580 images of 120 breeds of dogs. 
There are pictures of dogs of the same breed but of different colors, ages and sizes. In the examples below, a breed of dog called Japanese Spaniel is represented in 2 colors (black and white and brown and white) and in different ages. However, in some images there are not only dogs but also people. Also, some folders with photos of a certain breed included another breed. The examples below show photos of the Airedale breed. However, it's evident that the third dog is different from the others.



Description of the ML models you used with some theory 

	Convolutional Neural Network was mainly used for this project. It is a subset of the several artificial neural network models that are employed for various purposes and data sets. A CNN is specifically used for image recognition and pixel data processing activities. It is constructed of a number of different layers, including convolutional layers, pooling layers, and fully connected layers. There are different types of CNN models. For example: DenseNet, LeNet, AlexNet, ResNet, etc. In my project Alexnet was used. 
	
	Alexnet compared to the original LeNet, has many more filters, increasing the number of items it can classify. AlexNet architecture consists of 5 convolutional layers, 3 max-pooling layers, 2 normalization layers, 2 fully connected layers, and 1 softmax layer. Each convolutional layer consists of convolutional filters and a nonlinear activation function ReLU. Also, AlexNet uses "dropout" rather than regularization to address overfitting.
	
	All models (Sequential) and layers (2D convolution layer , MaxPooling2D, Dense, Flatten, Dropout) were taken from Keras. A CNN can be instantiated as a Sequential model because each layer has exactly one input and output and is stacked together to form the entire network. 
	2D convolution layer - creates a convolution kernel that is convolved with the layer input to produce a tensor of outputs.
	The largest or maximum value in each patch and the feature map is determined by the Keras MaxPooling2D pooling or max pooling procedure.
	The Dropout layer randomly sets input units to 0 with a frequency of rate at each step during training time, which helps prevent overfitting.






















Discussion

Critical review of results 

One of the disadvantages is that the model takes a very long time to train. However it shows good results in predicting the breed almost correctly at close range, taking into account that a particular breed can have several colors. But at a far distance, it is very difficult to correctly predict the breed of a dog.

Next steps 

Search for a solution to predict the breed of a dog from a long distance and for poor quality images. Improve accuracy.







References:

https://informburo.kz/interview/otkuda-berutsya-brodyachie-zhivotnye-i-pochemu-otstrel-eto-ne-vyhod

https://www.kaggle.com/datasets/jessicali9530/stanford-dogs-dataset

https://www.techtarget.com/searchenterpriseai/definition/convolutional-neural-network

https://www.geeksforgeeks.org/convolutional-neural-network-cnn-in-machine-learning/

https://iq.opengenus.org/different-types-of-cnn-models/

https://www.mygreatlearning.com/blog/alexnet-the-first-cnn-to-win-image-net/

https://keras.io/api/layers/convolution_layers/convolution2d/#:~:text=2D%20 convolution%20player%20

https://www.educba.com/keras-maxpooling2d/



