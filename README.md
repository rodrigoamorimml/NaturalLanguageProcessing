## Natural Language Processing Projects
---

#### In this repository i'll be describing and explaining a few **Natural Language Processing Projects** like:



- [ ] Sentimental Analysis using different tecniques of representation of text (Bag of Words, Word Embedding)
- [ ] Sentimental Analysis using some Deep learning architectures.
- [ ] Spam Detection Algorithm.
- [ ] An Auto Correct System.
- [ ] An Auto Complete System using N-Gram Language Model.

#### - *Sentimental Analysis using different tecniques of representation of text (Bag of Words, Word Embedding)*

The dataset that will be used in the first project is the Movie Review Dataset, this dataset is a collection of movie reviews from the 
IMDB website in the early 2000s by Bo Pang and Lillian Lee. The dataset is comprised with 1000 positive and 1000 negative movie reviews draw  from an archive of the rec.arts.movies.reviews newsgroup hosted by IMDB. The authors refer to this dataset as the *polarity dataset*.

This dataset can be download at:  [Moview Review Dataset Polarity](http://www.cs.cornell.edu/people/pabo/movie-review-data/review_polarity.tar.gz)

After unzipping the file, you will have a directory called txt sentoken with two subdirectories containing the text neg and pos for negative and positive reviews. Reviews are stored one per file with a naming convention from cv000 to cv999 for each of neg and pos.

For this example it's used the Bag of Words representation of text, this representation describes the occurence of a word within a document. This technique is built using two steps, first we need a vocabulary of known words (where this vocab can be using unique words or unique n-grams) and the second step is the measure of the presence of this words, where can be by:
  - Count
  - TF-IDF (Term Frequency - Inverse Document Frequency)
  - Frequency
  - Binary

Besides this, is shown the pre processing step, where we clean the data and tokenize the data (split the raw text into words and apply some integer values to them. ), this technique are widely used to get better model results.



#### - *Sentimental Analysis using some Deep learning architectures.*

This second example, we'll be using the the kaggle datasets Jig-Saw Toxic Comment for classification task  where can be found at: [Toxic Comment Dataset](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge).


This dataset contains differents types of toxic comments and the task it's to classify this comments in six possibles categories. Since a single comment can be placed in more than one category, then it'll be used 6 binary classification to complete this task. 

In addition it will be used different types of architeture of neural networks to compare their performance and accuracy in this dataset, like a  ConvNet and a Reccurent Neural Network.
Besides that, for the pre processing stage it will be used a Pre-trained Word Embedding Vector that can be download at: [Glove Embedding Vector](http://nlp.stanford.edu/data/glove.6B.zip)

#### - *Spam Detection Algorithm.*

In the third example, it's also used a kaggle dataset, the spam detection dataset, the dataset can be found at: [Spam Detection](https://www.kaggle.com/uciml/sms-spam-collection-dataset).

This dataset is a set of SMS tagged messages that have been collected for SMS Spam research. It contains one set of SMS messages in English of 5,574 messages, tagged acording being ham (legitimate) or spam. For this classification task it's used 2 types of neural network architectures, one Conv Net model and one RNN model, and using the same pre process step and the same optmizer and loss function, we compare the two models to see which one performs better.

#### - *An Auto Correct System.*

The forth project, We built from scratch an Auto Correct System, basically an auto correct system is an application that changes mispelled words into correct ones, as an example, is the phone spell corrector, where suggest options to correct a given word that the system thinks its mispelled. The application is divided is four parts, where we go through every part to explain and create a function that apply this step.

#### - *An Auto Complete System.*

The fifth example uses the same principle of the example above, we built from scrach an auto complete system, this system can be used is some task, like:
  - Web Searchs, when you looking for something, the model often have suggestion to help complete your search.
  - When you writing a email, you get suggestions of words to complete your sentence.
  
The The key behind the auto-complete system is a language model. A language model is a tool the calculates the probabilities of sentences and estimate the probability of upcoming word given a history of previous words.

A language model assigns the probability in a way that more likely sequences receive higher scores, as a example:
  - ''I have a car'' is expected to have higher probability than "I am a car", since the first sentence looks like more natural in the real word.

For this application we'll be using the language modeling method called N-grams, N-grams is a sequence of words (characters or other elements) where the order matters, as a example of N-grams, we have:
  - Unigram - Set of all unique words that appears in the text
  - Bigram - Set of all two words that appears side by side in the text
  - N-gram - Set of all n-words that appears together(with the correct order) in the text
