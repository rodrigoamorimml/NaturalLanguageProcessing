## Natural Language Processing Projects
---

#### In this repository i'll be describing and explaining a few **Natural Language Processing Projects** like:



- [ ] Sentimental Analysis using different tecniques of representation of text (Bag of Words, Word Embedding)
- [ ] Sentimental Analysis using some Deep learning architectures.
- [ ] Spam Detection Algorithm.
- [ ] An Auto Correct System.
- [ ] An Auto Complete System using N-Gram Language Model.



The dataset that will be used in the first project is the Movie Review Dataset, this dataset is a collection of movie reviews from the 
IMDB website in the early 2000s by Bo Pang and Lillian Lee. The dataset is comprised with 1000 positive and 1000 negative movie reviews draw  from an archive of the rec.arts.movies.reviews newsgroup hosted by IMDB. The authors refer to this dataset as the *polarity dataset*.

This dataset can be download at:  [Moview Review Dataset Polarity](http://www.cs.cornell.edu/people/pabo/movie-review-data/review_polarity.tar.gz)

After unzipping the file, you will have a directory called txt sentoken with two subdirectories containing the text neg and pos for negative and positive reviews. Reviews are stored one per file with a naming convention from cv000 to cv999 for each of neg and pos.

For this example it's used the Bag of Words representation of text, this representation describes the occurence of a word within a document. This technique is built using two steps, first we need a vocabulary of known words (where this vocab can be using unique words or unique n-grams) and the second step is the measure of the presence of this words, where can be by:
  - Count
  - TF-IDF (Term Frequency - Inverse Document Frequency)
  - Frequency
  - Binary
