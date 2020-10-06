# NLP-Search-Optimisation-for-Research-Papers
### Technology Used:
Text Summarization & Named Entity Recognition

### Abstract:
We are optimizing searches of educational texts with providing a brief summary containing the gist of the whole text as well as custom named entity tagging for efficiently relating the educational text with appropriate keywords. Here we use extractive summarization over abstractive summarization because in abstractive summarization there is a chance that the new sentences generated alter the meaning of the text. In extractive summarization important sentences are filtered for summarization.The custom NER will help us identify keywords which answers questions such as “ Which subject ?”, “Which domain ?”, “Who’s the author?”, etc.


### Project Introduction: 
While working on projects, we often face problems searching for the correct resources. With an incredible amount of educational resources available out there, it becomes tough to find the one matching your needs. To optimize searches of the correct resources and educational texts, we would like to come up with a product that effectively summarizes text and tag the text with the most weighted entities.
Here we will use extractive summarization as extractive methods attempt to summarize articles by selecting a subset of words that retain the most important points. To do so we take input of the technical text, then convert paragraphs into a list of sentences. The next and most important step is text processing, we cleanse the text by removing stop words according to the Spacy module and tokenize the sentence. After this, we need to evaluate the occurrence frequency of each token.  For the actual summarization, there are numerous methods such as seq2seq, variants to RNNs, and LSTMs. In this version, we will be using a custom attention mechanism to do the summarization. Compared to general techniques, instead of looking at all the words in the source sequence, we can increase the importance of specific parts of the source sequence that result in the target sequence with having an attention mechanism. For this project, we will use global attention. Here, the attention is placed on all the source positions.
In this next part, we will find custom-named entities from the summarized text like related technologies, authors, conferences, etc. These entities will be tagged to the text to make searching for these resources easier for the user. Since there are not many useful technical terms based NER, we will make our own custom model using tools provided by the Spacy library.


### Tech-Stack: 
Python (coding language), NLTK (library), Spacy (library), Streamlit (web interface).
