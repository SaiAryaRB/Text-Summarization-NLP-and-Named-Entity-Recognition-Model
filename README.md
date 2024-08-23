# Text Summarization NLP and Named Entity Recognition Model 

This Repository consists of two jupyter notebooks - TextSummarizationandNER and TextSummarizationAttempt

The first Notebook - TextSummarizationandNER uses the dataset conll2012_ontonotesv5-english_v12 from the Library datasets
to make a model for Named Entity Recognition that can capture Entities such as Person, Location, Language , Product and so forth
The model can distinguish between the Beginning of an entity and the inside of an entity
We have used a Bidirectional Long Short Term memory model to improve contextual understanding, along with an ADAM optimizer and the loss function used here is Cross-Entropy Loss

For text Summarization , we have used a pretrained model from the Transformers Library called BART , aand since BART works optimally with an input size of 1024 characters
we have split up input text into chunks of 1024 characters

The model inputs a PDF using pyPDF library and performs text summarization on it , then performs Entity Recognition on the Summarized Text . Using the Entities , we scrape youtube using these entitites as searchwords and generate the top 3 youtube Links 
These youtube links will provide visual aids that could help in Studying or other purposes

The Second Notebook - TextSummarizationAttempt is an NLP built from scratch that uses the dataset - gopalkalpande/bbc-news-summary. It uses a Sequence to Sequence Encoder Decoder Model to perform text Summarization . However , due to Lack of computational Resources this does not function accurately.



