# H.P. Lovecraft style Text Generation 

## ABOUT
The main idea of the project was to use Artificial Intelligence techniques to create the tool that would imitate the Lovecraft's
writing style to generate further sentences. 
In the area of Unsupervised Learning and NLP (Natural Language Processing), the Recurrent Neural Networks have been widely used, as they are great in analyzing the sequences, in this case sentences from the author's stories.
RNN was built with two bidirectional LSTM (Long-Short Term Memory) layers and trained for less than 100 epochs, reaching the accuracy around ~93.5%.


## User interaction
All you have to do to check how the model works, is to execute first two cells to load all necessary packages and the helper function,
that is actually responsible for generating the further text. Then, move to the last part of the notebook "Generating the text", load the serialized model and the tokenizer objects and execute the function. 


## Project files:
- Text Generation RNN.ipynb - the main file
- model.h5 - pretrained, ready to use RNN model to generate the sentences
- tokenizer.pickle - serialized tokenizer object, containing a set of all the words on which the model was trained on
- The Complete Works of H.P. Lovecraft.pdf - the pdf file, over 700 pages of the Lovecraft's stories, from which less than 200 was picked
to succesfully train the Neural Network.


## Dependencies:
numpy == 1.19.5
pandas == 1.1.5
matplotlib == 3.2.2
sklearn == 0.22.2
keras == 2.4.3
tensorflow == 2.4.1
PyPDF2 == 1.26.0
