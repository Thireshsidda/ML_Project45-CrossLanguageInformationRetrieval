# ML_Project45-CrossLanguageInformationRetrieval

### Cross-Language Information Retrieval System (CLIR)
This project implements a CLIR system that translates German queries into English and retrieves relevant documents from an English corpus.

### Project Goals:
Build a robust CLIR system using word-based translation and Okapi BM25 for information retrieval.

Evaluate the system's performance using standard IR metrics.

### Data Used:
bitext.(en,de): Parallel corpus of English and German sentences for training translation and language models.

newstest.(en,de): Separate parallel corpus for evaluating the translation system.

devel.(docs,queries,qrel): Documents in English, German queries, and relevance scores for each query-document pair.

### System Components:
##### Information Retrieval:
Implements BM25 model for ranking documents based on their relevance to a query.

Includes document loading, tokenization, preprocessing, TF-IDF representation, inverted index construction, and BM25 ranking.

##### Query Translation:
Employs a noisy channel model combining a language model with a translation model.

Utilizes unigram and trigram language models built from the bitext data.

Incorporates Add-k and Katz-Backoff smoothing for handling unknown words.

Evaluates language model performance using perplexity.

### Code Structure:
The code is well-organized and modular, with clear separation of concerns for each component.

File paths are stored in variables for easy access.

Text handling includes encoding detection and tokenization.

### Next Steps:
Implement the translation model within the noisy channel framework.

Integrate the translation and retrieval components to form the complete CLIR system.

Evaluate the system's performance using standard IR metrics like MAP and NDCG on the devel dataset.


### Additional Notes:
This project provides a solid foundation for building a CLIR system.

Feel free to explore further enhancements and optimizations for improved performance.

