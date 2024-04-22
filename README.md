# Yelp FastText Word Embeddings Comparison

This project aims to compare word embeddings generated using a custom FastText model trained on Yelp dataset with embeddings generated using a pre-trained FastText model from Facebook. 

## Steps

1. **Yelp Dataset:**
   - Download the Yelp dataset.
   - Or use it from kaggle directly

2. **Data Selection:**
   - Choose as many records/sentences as needed from the "text" attribute.

3. **Preprocessing:**
   - Apply the same preprocessing steps Cleaning Data: Eliminates any symbols or characters that are not relevant to the text content. Normalization: Converts all text to lowercase to 
    ensure uniformity for subsequent processing steps. Tokenization: Splits the text into individual words or tokens, facilitating further analysis. Lemmatization or Stemming: Reduces 
    words to their base or root form to standardize variations of the same word. Users can choose between lemmatization or stemming based on their preference or requirements. Stop Words 
    Removal: Filters out common words such as "is," "and," "the," etc., which do not add significant meaning to the text. Unique Word Extraction: After processing, the script outputs all 
    unique words present in the text data. This ensures that only distinct words are considered for analysis, providing valuable insights into the vocabulary used in the text..

4. **FastText with Gensim:**
   - Utilize the Gensim library to use FastText.
   
5. **Training Custom FastText Model:**
   - Train a FastText model on the preprocessed training data.

6. **Load Pre-trained Model:**
   - Load a Facebook pre-trained FastText model. 

7. **Select Random Words:**
   - Choosen 20 random words from the words in the training data.


8. **Find Similar and Dissimilar Words:**
   - For each randomly chosen word, find the top 10 similar and dissimilar words using both the custom-trained model and the pre-trained model.

9. **Generate Report:**
    - Compile all the results obtained into a PDF.
    - Write a conclusion about which model performs better.

## How to Use

1. Clone this repository:

   ```bash
   git clone https://github.com/Samahussien7/fastText-Model.git
   ```

2. Follow the steps mentioned above.

3. Run the Python script provided in this repository.

## Dependencies

- Python 3.x
- Gensim
- FastText

