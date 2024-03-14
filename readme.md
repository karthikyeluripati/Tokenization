# Tokenization

1. Tokenization and Normalization
2. Part-of-Speech Tagging
3. N-Grams

Let's discuss each question based on the provided code and output:

### tokenizing by word versus by sentence

- Tokenizing by word (`tokens_word`) produces a list of individual words.
- Tokenizing by sentence (`tokens_sentence`) gives a list of sentences.
- The choice of tokenization method depends on the level of granularity needed for analysis. Tokenizing by word is more fine-grained, while tokenizing by sentence provides a broader context.

### Pos_tag()
- The `pos_tag()` function was used to tag each tokenized word with its part-of-speech.
- Common POS tags observed in the output include:
  - Most frequent: 'NN' (Noun).
  - Least frequent: VBP (sing. present, non-3d).
- Errors:
- The word "processing" in the given text is tagged as a gerund or present participle (VBG) when part-of-speech tagging is applied. But Here in the output we got NN as output

### bi-gram and tri-gram
- The code used `ngrams()` and `FreqDist()` to identify the most common bi-grams and tri-grams.
- Most common bi-grams and tri-grams reveal key phrases or concepts in the text. They provide insights into recurring combinations of words.
- For example, if a common bi-gram is 'natural language,' and a common tri-gram is 'machine learning approaches,' it suggests that the text discusses natural language and machine learning. 
