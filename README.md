# Text_Generation
Neural Network Model for Text generation

A language model can predict the probability of the next word in the sequence, based on the words already observed in the sequence.
The Republic is the classical Greek philosopher Plato’s most famous work. It is structured as a dialog (e.g. conversation) on the topic of order and justice within a city state The entire text is available for free in the public domain.

In this Project, we will develop a model of the text that we can then use to generate new
sequences of text. The language model will be statistical and will predict the probability of
each word given an input sequence of text. The predicted word will be fed in as input to in
turn generate the next word.

There is no correct answer. With enough time and resources, we could explore the ability of the model to learn with differently sized input sequences. Instead, we will pick a length of 50 words for the length of the input sequences, somewhat arbitrarily.

The model is compiled specifying the categorical cross entropy loss needed to fit the model.Technically, the model is learning a multiclass classification and this is the suitable loss function for this type of problem. The efficient Adam implementation to mini-batch gradient descentis used and accuracy is evaluated of the model.

Finally, the model is fit on the data for 5 training epochs with a modest batch size of 128 to speed things up.
I cannot use 100 epochs due to system constraints.

we will get different results, but perhaps an accuracy of just over 50%(When using 100 epochs) of predicting the next word in the sequence, which is not bad.
