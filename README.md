The model which is created is used to convert human readable dates like "April 20 1999" to "1999-04-20".
It was created using Attention mechanism wherein the output depends only on certain regimes of the input to generate a character of an ouput.
The dates were generated using the faker module, where we run through a loop to get the required dataset.
The characters of both the dates(human readable and machine readable) were mapped to integers in a dictionary which was further used to preprocess the dataset where we convert the dataset to a one-hot encoding
This model was created using the Attention mechanism with the pre-activation being a bidirectional LSTM and the post activation layer being unidirectional LSTM.
The weights alpha(the attention paid at timestep t to generate the output characer was calculated using activations from both pre-attention and post-attention.
The attention can be seen in the generated plot in the code.
