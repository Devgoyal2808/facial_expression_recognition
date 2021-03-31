# facial_expressions
A set of images for classifying facial expressions.Dataset of different facial expressions ['anger','surprise','disgust','fear','neutral','happiness','sadness','contempt'] used for training machine learning algorithms.
Dataset forked from : https://github.com/muxspace/facial_expressions

# Model for predicting facial expressions
Convolutional Neural Network model is built using Keras.

Model Layers are as follow:

2D Convolutional Neural Network Layer with 16 units with stride 3,3                                                                                                                
2D Maximum Pooling Layer which convert matrix of m*n to (m/2)*(n*2) taking max((i,j),(i+1,j),(i,j+1),(i+1,j+1))                                                                     
2D Convolutional Neural Network Layer with 32 units with stride 3,3                                                                                                                 
2D Maximum Pooling Layer which convert matrix of m*n to (m/2)*(n*2) taking max((i,j),(i+1,j),(i,j+1),(i+1,j+1))                                                                     
2D Convolutional Neural Network Layer with 64 units with stride 3,3                                                                                                                 
2D Maximum Pooling Layer which convert matrix of m*n to (m/2)*(n*2) taking max((i,j),(i+1,j),(i,j+1),(i+1,j+1))                                                                     
A Flatting layer which adds an extra dimension in data from (shape,) to (shape,1)                                                                                                   
A simple Neural Network Layer of 1024 units with 1024 bias and activation relu                                                                                                     
The final output layer with units equal to number of output possible and softmax activation function.                                                                                

The Model predict the facial expressions of the photos in dataset.
