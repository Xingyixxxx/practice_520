
# Code Filling Assignment

## Blank 1

```python
#convert training data into vectors in Bow
bow_vectorizer, bow_train_features = bow_extractor(train_X)
bow_test_features = bow_vectorizer.transform(test_X)
```

## Blank 2

```python
#convert training data into vectors in Tfidf
tfidf_vectorizer, tfidf_train_features = tfidf_extractor(train_X)
tfidf_test_features = tfidf_vectorizer.transform(test_X)
```

## Blank 3

```python
#enter some new data to feel the accuracy of the program
input = final_test()
    
bow_input_features = bow_vectorizer.transform(input)
tfidf_input_features = tfidf_vectorizer.transform(input)
print('bow input predictions: ',mnb_bow.predict(bow_input_features))
print('tfidf input predictions: ',mnb_tfidf.predict(tfidf_input_features))
```

## Function `final_test`

> A new function was written to implement the test code

- The test data is in CSV format
- Reads the CSV and extracts the Chinese content
- Randomly selects 10 samples from the test set
- Displays the test samples before testing
