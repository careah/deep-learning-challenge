# deep-learning-challenge

1. The target variable for the model is "IS_SUCCESSFUL." This variable represents whether a charity donation was successful or not.

2. The feature variable includes all columns in the dataset except for "IS_SUCCESSFUL." These features are used as input to the neural network to predict the target variable.

3. The Removed variables are "EIN" and "NAME" columes as they are identifies and not related to the prediciton. 

For the original model, I selected the following: 
Hidden Layer 1: 8 neurons with ReLU activation function.
Hidden Layer 2: 5 neurons with ReLU activation function.
Output Layer: 1 neuron with sigmoid activation function.

Optimization 1:
Hidden Layer 1: 12 neurons with ReLU activation function.
Hidden Layer 2: 8 neurons with ReLU activation function.
Output Layer: 1 neuron with sigmoid activation function.

Optimization 2:
Hidden Layer 1: 60 neurons with ReLU activation function.
Hidden Layer 2: 40 neurons with sigmoid activation function.
Hidden Layer 3: 10 neurons with hyperbolic tangent (tanh) activation function.
Hidden Layer 4: 5 neurons with softmax activation function.
Output Layer: 1 neuron with sigmoid activation function.

Optimization 3:
Hidden Layer 1: 40 neurons with ReLU activation function.
Hidden Layer 2: 20 neurons with sigmoid activation function.
Hidden Layer 3: 5 neurons with ReLU activation function.
Output Layer: 1 neuron with sigmoid activation function.

I was not able to achieve teh target model performance with this model. In each attempt the number of neruons in hidden layers was adjusted, activation function was changed, and a different layer architecture was adjusted. I also used callbacks to save model weights during training, and checkpointing to prevent overfitting, and scaled the data using StandardScaler and I still was unable to get the accuracy over 75%.

The attempted deep learning models, though a combination of adjustments it demonstrated modest accuracy and loss in predicting charity donation success, and although 72% is still high, it's not 100%.