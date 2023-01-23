#### **Natural Language Processing**

This is all about the basics of natural language processing, techniques used to vectorize text, and its application to sentiment analysis using neural network.

First, run the command to install repository requirements:
`pip install - r requirements.txt`

Read (or run) the notebooks according to this order:

1. nlp
2. tfidf
3. word_embeddings
4. document_embeddings
5. contextual_embeddings
6. evaluation-of-techniques
7. tweets-ann-torch_2
8. tweets-ann-autoencoder
9. tweets-ann-balanced

Tokenized tweets and the target variable array are stored in `notebooks/csvs`.

Feature vectors will be saved in `notebooks/vectors`, although only the output vector from `TfidfVectorizer` is stored, and all others are ignored because of their size. Nonetheless, all these vectors will be stored in that said folder.

Torch Models will be saved in `notebooks/torch_models`:

1. `model_0.pth` - contains the model trained and tested on the **validation set**
2. `model_1.pth` - contains the model trained using the hyperparameters found from validation and tested on the **test set**
3. `model_2.pth` - contains the model trained from a `~balanced` dataset and tested on the same **test set** used on `model_1`
4. `variational-autoencoder.pth` - contains the variational autoencoder which was trained on the `negative` class, to resample it and make it equal to the average of the population of the `neutral` and the `positive` class

Much of the explanations are in `markdown` cells of each notebook, obtained from resource articles found in the Internet, valuable videos from Youtube, distilled to the interpretation of the author. This is to provide a detailed and comprehensive understanding of the topics.

Take note that the author is _generally new_ with natural language processing and was also learning while writing the `notebooks`.

Pictures attached are from the word document `Feature Extraction Techniques.docx` which is also available with this repository.

This repository serves as a partial requirement to a project administered by Mr. Raphael Alampay, but also as a valuable resource for the author and to the readers.

Thank you!
