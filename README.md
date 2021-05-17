# BERT
Bidirectional Encoder Representations from Transformers is a Transformer-based machine learning technique for natural language processing pre-training developed by Google.<br> 
BERT makes use of Transformer, an attention mechanism that learns contextual relations between words (or sub-words) in a text. In its vanilla form, Transformer includes two separate mechanisms — an encoder that reads the text input and a decoder that produces a prediction for the task. Since BERT’s goal is to generate a language model, only the encoder mechanism is necessary. The detailed workings of Transformer are described in a paper by Google.

As opposed to directional models, which read the text input sequentially (left-to-right or right-to-left), the Transformer encoder reads the entire sequence of words at once. Therefore it is considered bidirectional, though it would be more accurate to say that it’s non-directional. This characteristic allows the model to learn the context of a word based on all of its surroundings (left and right of the word).<br>

Instead of predicting the next word in a sequence, BERT makes use of a novel technique called Masked LM (MLM): it randomly masks words in the sentence and then it tries to predict them. Masking means that the model looks in both directions and it uses the full context of the sentence, both left and right surroundings, in order to predict the masked word. Unlike the previous language models, it takes both the previous and next tokens into account at the same time. The existing combined left-to-right and right-to-left LSTM based models were missing this “same-time part”. (It might be more accurate to say that BERT is non-directional though.)

What is BERT used for?<br>
BERT is currently being used at Google to optimize the interpretation of user search queries. BERT excels at several functions that make this possible, including:

Sequence-to-sequence based language generation tasks such as:<br>
Question answering<br>
Abstract summarization<br>
Sentence prediction<br>
Conversational response generation<br>

Natural language understanding tasks such as:<br>
Polysemy and Coreference (words that sound or look the same but have different meanings) resolution<br>
Word sense disambiguation<br>
Natural language inference<br>
Sentiment classification<br>
