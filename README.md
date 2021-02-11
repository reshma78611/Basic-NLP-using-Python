# Text Processing/NLP using Python

Text Processing is one of the most common task in many ML applications. Below are some examples of such applications.

• Language Translation: Translation of a sentence from one language to another.\
• Sentiment Analysis: To determine, from a text corpus, whether the  sentiment towards any topic or product etc. is positive, negative, or neutral.\
• Spam Filtering:  Detect unsolicited and unwanted email/messages.

## Natural Language Processing:

Transforming text into something an algorithm is a complicated process. We will see basic Preprocessing Operations in this repository.

**Data Preprocessing:**

Basic Data preprocessing steps of text data are:

  1. Tokenization — convert sentences to words
  2. Removing unnecessary punctuation, tags
  3. Removing stop words — frequent words such as ”the”, ”is”, etc. that do not have specific semantic
  4. Stemming — words are reduced to a root by removing inflection through dropping unnecessary characters, usually a suffix.
  5. Lemmatization — Another approach to remove inflection by determining the part of speech and utilizing detailed database of the language.
  
After Data Preprocessing, we will go with Feature Extraction.

**Feature Extraction:**

In text processing, words of the text represent discrete, categorical features. How do we encode such data in a way which is ready to be used by the algorithms? The mapping from textual data to real valued vectors is called feature extraction.

One of the simplest techniques to numerically represent text is *Bag of Words.*

   **1. Bag of Words**\
            - Focuses all the words in corpus and its frequency\
            - Throws away all order information.\
            *Limitations:*\
            - Can't account for position.\
            - Cant account for context.\
            - Cant completely capture importance of words\
    **2. TF-IDF**\
            *TF*\
            - Term Frequency\
            - Number of repetitions of a word in a document/Total number of words in a document\
            - Captures importance of a word in a document.\
            *IDF*\
            - Inverse Document Frequency\
            - log(number of documents)/(number of documents containing the word)\
            - Captures importance of a word in entire corpus\
            *Limitations:*\
            - One of the major disadvantages of using TF-IDF is that it discards word order thereby ignoring the context and in turn meaning of words in the document.\
            
            
  For natural language processing (NLP) maintaining the context of the words is of utmost importance. To solve this problem we use another approach called Word Embedding.
  
   **3. Word Embedding:**
   
        It is a representation of text where words that have the same meaning have a similar representation. In other words it represents words in a coordinate system where related words, based on a corpus of relationships, are placed closer together.
        One of the word embedding method is Word2Vec.
        
        
   ***Word2Vec:***

       Word2vec takes as its input a large corpus of text and produces a vector space with each unique word being assigned a corresponding vector in the space. Word vectors are positioned in the vector space such that words that share common contexts in the corpus are located in close proximity to one another in the space.  For example, man is to woman as uncle is to ? (aunt) using a simple vector offset method based on cosine distance.
       
       
 ## Programming:
            Python
            
 **The Codes regarding NLP with Pre-processing methods such as *Tokenization, Stemming, Lemmatization, stopwords, Bag-of-words, TF-IDF, Word2Vec* are discussed in this repository in detail**
       
       
  
    
