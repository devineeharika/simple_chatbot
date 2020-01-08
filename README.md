# simple_chatbot
basically chatbots are 2types
a)retrieval based chatbot:
          it uses pre-defined input patterns and responses it uses heuristic approach to find responses.
b)generative based chatbot:
          they are based on seq2seq neuralnetworks.
 it will be using intents.json file as a dataset
 Words.pkl – This is a pickle file in which we store the words Python object that contains a list of our vocabulary.
Classes.pkl – The classes pickle file contains the list of categories.
Chatbot_model.h5 – This is the trained model that contains information about the model and has weights of the neurons.
we need tokenize patterns,then lemmatize and remove duplicate words.
we need to create training data
like it is text so we need to convert into numbers.
create our bag of words array with 1, if word match found in current pattern
output is a '0' for each tag and '1' for current tag (for each pattern)
Create model - 3 layers. First layer 128 neurons, second layer 64 neurons and 3rd output layer contains number of neurons
equal to number of intents to predict output intent with softmax
Compile model. Stochastic gradient descent with Nesterov accelerated gradient gives good results for this model
