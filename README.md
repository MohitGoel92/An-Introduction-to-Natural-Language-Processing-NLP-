# An Introduction to Natural Language Processing (NLP)

This repository is used to take a complete NLP novice to a level of business proficiency. We will be introduced to Natural Language Processing (NLP) and will build our knowledge to the point where we are comfortable undertaking business projects. Listed below are the topics we will cover:

- Section 1: Introduction to Natural Language Processing
- Section 2: Natural Language Processing pipelines for text analysis
- Section 3: Information extraction for NLP tasks.
- Section 4: Applications of NLP, libraries and methods.
- Section 5: Building NLP pipelines with Python.

## Section 1: Introduction to Natural Language Processing

In this section we will cover:

- What NLP is, the basic tasks of NLP and why is it an important skill to have?
- What are the most common use cases of NLP in the industry (in modern computer systems and applications).
- What are the most common data sources?
- Python programming basics.
- Introduction to Python Natural Language Toolkit (NLTK).

### What is NLP?

- Natural Language Processing (NLP) primarily deals with interactions between humans and computers. The main aim here is to process, interpret and analyse natural language data.
- Common NLP challenges that industries face are:
    - Speech recognition.
    - Text understanding.
    - Natural Language Generation.

Examples of NLP include Siri (Apple), Whatsapp, and Alexa (Amazon). So in essence, NLP is a software for speech recognition, language understanding and analysis, dialogs, and speech to text. In NLP, text is treated as raw data that is usually unstructured. For instance, a report, email, review or complaint. An NLP program analyses and presents results in an automated way. As NLP programs aim to perform tasks based on understanding human langauge, the program is able to extract information from text.

NLP makes human to machine interactions easy.
- NLP is a way to support human to machine communication.
- Data mining: Identify hidden meaning and patterns of natural language data in an automated way.
- Information extraction: Extracting useful information from text such as names, locations, telelphone numbers ... etc.

Why is NLP important?

- Interpretation and manipulation of language is a key challenge for modern industries.
- A lot of text data is generated daily, making automated analysis a key task.
- Human language understanding NLP tasks for:
  - Reading text
  - Writing text
  - Speaking text
  - Listening text

Obstacles to NLP

- Exploring the meaning and relationships of languages to cognition and meaning of text was always a challenging task for scientists.
- Understanding natural language is already a difficult task for humans, let alone machines. This is because languages can have a very ambiguous nature. For instance, "You know Tom", and "You know Tom?".
- Personal styles and many different ways of expressions. For instance, "OK :)", and "OK :(".
- Many different languages and colloquial styles.

A simple NLP solution to a problem is categorising emails into "Inbox" or "Junk". This is performed by seeking particular words or a combination of words and probabilistically deeming it as useful or spam. The classification uses a large dataset of already labelled emails as a guide to categorising the new or incoming emails. Phrases like "best price", "cash bonus", "earn money", "you won £1 million" ... are all triggers that will classify the email as spam. This is also know as **Text Classification**.

NLP uses a Corpus as the basis of its analysis.

**Corpus:** A huge collection of written data. In our case of email classification, these are the emails that are already classified and labelled as spam or ham.

Below is a basic outline of an NLP task:

- Preparing the text data for analysis.
- Creating dictionaries of words and frequencies.
- Feature extraction process.
- Training a classifier to predict the class of new emails.

Data is constantly being generated, for instance, social media (Twitter, Facebook, Whatsapp ... etc). Common use cases of NLP include:

- Chatbots: Heavily used for businesses such as customer services. If you type in "Hello", the NLP program analyses the text and will reply "Greetings!". NLP is used to map text to meaningful insights capable of responding to written commands. For instance, typing in a request and the system providing you with the required data.
- Sentiment Analysis: Here NLP identifies and classifies the emotions within a text using text analysis methods. For instance, understanding the reviews for a restaurant and whether they are positive or negative.
- Creditworthiness Assessment: A.I. algorithms analyse text and provide credit scores as predictive analytics for banks. Banks use alternative data sets for scoring potential borrowers, for instance, social media posts, internet activity, and online behaviour. This takes the following process:
    - Mining the web for information on potential customers.
    - Analysing the data and providing assessments of the customers creditworthiness.
    - Banks use trained datasets that are prelabelled indicating the level of risk for a customer.
- Hiring and Recruitment: NLP is changing the way HR operate. Traditionally, recruiters need to review thousands of CV's for a single job post which can takes hours and hours of navigating emails. NLP can support this process by analysing candidate reports and scoring them against standard datasets. This provides indications for top candidates, removing bias and increasing diversity.
- Healthcare: Medical professionals and institutions now communicate with patients electronically. For example via email, online forms with symptoms and online video consultations. Despite the already overwhelming amount of medical terms and medications pharmacists have to keep track of, in a global world language barriers add more complexity to this hurdle. NLP has been proven to assist in the healthcare sector. For instance, researchers from the University of Alabama found that NLP identification of reportable cancer cases was 22.6% more accurate than the manual review of electronic health records (EHR). NLP helps extract useful data from EHRs and even give EHRs indications and alters to prevent human errors. In other words, NLP helps with increasing acccuracy.

NLP uses a variety of data including:

- Structured data:
    - Data that has been organised and includes a clear data model.
    - Data in relational databases that represent a table with rows and columns (SQL).
    - Robust, easy to manage and control.
    - Less flexible as it follows a particular data model, and less scalable.
    - According to industry estimates, only 21% of the available data is present in a structured form.
- Semi-structured data:
    - Data has a level of organisation and structure that makes easy analysis, or gives indications how to analyse.
    - An XML format is an example of this category.
    - More flexible than structured data and easy to scale.
    - There is a schema indication, but users have the freedom to alter it.
- Unstructured data:
    - Data is not organised and there is no predefined data model.
    - Different formats include text files, such as Word documents, logs and PDF reports.
    - Absence of schema makes it scalable and flexible.
    - Difficult to analyse and process as it's based on character based analysis.
    - Mining unstructured data provides new insights and uncovers unknown information hidden in data. We can detect patterns and trends, and relationships and connection of unrelated data.

NLP is about user generated information:

- Emails
- Word processing documents
- Presentations
- Logs and reports
- Audio and video files
- Social media posts

**NLTK:** The Natural Language Toolkit has the most common tools for NLP. Using NLTK we can build Python programs to work with human language data. Huge collection of datasets and corpra and lexical resources. The NLTK library provides us with almost all the tools we need to analyse text.

### Python Refresher

We will quickly refresh our Python skills so we can move on smoothly with this course.

Exercise: Run the code that counts all the cells in the following string, "Romeo and Juliet.".

Solution:

```
text = """Romeo and Juliet."""

counter = 0
for x in text:
    counter = counter + 1 #or we can have counter+=1
print(counter)
```
The below summarises basic Python conditionals:

```
x = -9

if x>0:
  print('Positive number')
elif x<0:
  print('Negative number')
else:
  print('zero')
```

Loops help you execute blocks of code repeatedly.

```
items = ["book","pen","eraser"]
for x in items:
  print(x)
```

```
i = 0
while i<5:
  print(i)
  i+=1
```

**Python lists:** A python list is a collection of data that is ordered and changeable, and allows duplicate members.

- Strings in Python are lists of bytes that repesent Unicode characters.
- The following code represents two ways of creating a text variable in Python. In our cases, both variables are the same.

```
nameString = "Mary"
nameArray = ["M", "a", "r", "y"]
```

The following code creates a list of items and prints the list:

```
items = ["book","pen","eraser"]
print(items)
```

**Python Dictionary:** A dictionary is a collection which is unordered, changeable and indexed. Dictionaries differ from lists primarily in how elements are accessed. List elements are accessed by their position in the list via indexing.

```
mydata = {
    "nombre":"Mary",
    "ciudad":"Londres",
    "ano": 1992
}
print(mydata)
print(mydata['ciudad'])
```

The output to the below will be 34

```
dict1 = {"name":"Mary", "age":34, "city":"London"}
print(dict1["age"])
```

**Python Functions:** A function is a block of code that we call in programs and use it to run modular and repeated tasks.

```
def function(x):
  return x ** 2 # A number to the power of 2
print(function(-9)) # we must call the function name, which is function
```

A function returns a value back to the user, and the user decides how to further proceed with this. A function that does not return a value is called void.

```
# Function for counting the number of characters in a string

def cc(strings):
  counter=0
  for x in strings:
    counter+=1
  print(counter)

cc("Message Mensaje Letter Carta")
```

```
# The function below returns a string as a list of words

text = "She sells sea shells on the sea shore"

def splitter(atext):
  return atext.split()

print(splitter(text))
```

```
# The function below counts how many instances a word exists in a given phrase. 
# After, we will call the function to lookup the number of instances the word sea exists in the text variable.

text = "She sells sea shells on the sea shore"

def count_words(atext,lookup):
  counter_lookup=0
  for x in splitter(atext):
    if x == lookup:
      counter_lookup+=1
  return counter_lookup

print(count_words(text,"sea"))

# In our case, the output will be 2.
```

In the below, we are using a "Boolean" variable (True or False) as a return value. The below will print True.

```
text = "She sells sea shells on the sea shore"

def search_word(atext,lookup):
  for x in splitter(atext):
    if x == lookup:
      return True
  return False

print(search_word(text,"sea"))
```

**Python Tuples:** A tuple is a collection which is ordered and unchangeable. In Python, tuples are written with round brackets.

```
tuple = ("uno","dos","tres","cuatro")
print(tuple)
```

**Python Sets:** Sets are unordered and unindexed, with elements that are unique. Therefore, any repeated elements will only be printed out once. Elements in the set can be changed, unlike tuples. In Python, sets are written with curl brackets.

```
set = {"Gris","Azul","Rojo"}
print(set)
```

Let us use NLP to create a word frequency program using dictionaires.

```
corpus = "London is the capital of England . London is also the financial hub . Birmingham is the second largest city in England , after London ."

# Create an empty dictionary

word_freq = dict()

# Transform the corpus to a string and then split the corpus variable to words

corpus_word = str(corpus).split()
for x in range(len(corpus_word)):
  if corpus_word[x] not in word_freq:

# Create a key for each word and a counter as a value, then increase a counter as many times as the word appears in the text.

    word_freq[corpus_word[x]] = 1
  else:
    word_freq[corpus_word[x]]+=1
print(word_freq)
```

**NLTK**

- NLTK comes with many corpora, trained models ... etc
- In our case, we need to use the word_tokenize Python method, that in turn requires the pre-trained Punkt tokenizer.

```
import nltk
nltk.download('punkt')
sentence = "NLTK for life!"
tokens = nltk.word_tokenize(sentence)

print(tokens)
```

The following code installs the NLTK library onto the Colab Notebook. The code will also download a book collection to use as a dataset for learning NLTK.

```
import nltk
nltk.download('book')

from nltk.corpus import brown
brown.words()
```

The following code will download a book collection to use as a dataset for learning NLTK. This will output a selection of books for us to use.

```
from nltk.book import *

# The below will allow us to load Moby Dick by Herman Melville.

text1
```

*Concorance* permits us to see words in context, so we can examine the richness and diversity of a language. For instance, we can look for the context of the word "sense" in the Moby Dick by using the below.

```
text1.concordance("sense")
```

*Similar* extracts words that appear in a similar range of context with the word affection.

```
text1.similar("affection")
```

*Collocations* refer to a word or phrase that is often used with another word or phrase, in a way that sounds correct to people.

```
text1.collocations()
```

### Summary

In the section, we covered:

- Natural Language Processing (NLP) and the basic concepts behind it.
- NLP and datasets by focusing on textual data.
- How to build NLP pipelines to analyse text in series of steps.
- We reviewed Python and some fundamental aspects.
- We introduced the Python Natural Language Toolkit (NLTK):
    - We ran some basic analytics.
    - We developed our first pipeline.

## Section 2: Natural Language Processing piplelines for text analysis

In this section we will cover:

- Introduction to Neural Language Processing corpa.
    - Gutenberg, Brown, Reuters, Inaugural, ... etc.
- Working with raw text.
    - Regular expressions with Python regex library.
- Building an NLP pipeline.
- Word segmentation for different languages.
- Introducing SpaCy library.
- Developing an NLP Pipeline with Python.

### Introduction to NLP Corpora

- NLP programs heavy or linguistic datasets are known as **corpora**.
- A **corpus** is a collection of texts used in machine learning tasks.
    - Data is usually labelled and presented in a way to assist other NLP tasks.
- NLTP provides a selection of corpora for us to explore.
- In the previous section, we used predefined texts using the following code:
```
from book import *
```

### Using the Gutenberg Corpus

- The project Gutenberg electronic archive contains 25,000 free electronic books.
- Let us work with the Gutenberg corpus and load the NLTK package:
```
import nltk
nltk.download('gutenberg')
nltk.corpus.gutenberg.fileids()
```

### Using the Gutenberg Corpus (txt files)

- We can start working with the shakespeare-hamlet.txt corpus and try to run some simple analytics.
- similarly, we can open any txt text and use NLTK to prepare it for analytics.
```
hamlet = nltk.corpus.gutenberg.words('shakespeare-hamlet.txt')
```
- The code loads the hamlet text as a Python list so its quite easy to run simple Python commands, such as len() method to extract the length of the text (words).
```
hamlet_len = len(hamlet)
```
- The above will print 37,360 words.
- Let us use the cocordance method (from the previous section).
```
hamlet = nltk.Text(hamlet)
hamlet.concordance('King')
```

### Counting words using NLTK and a corpus

- Let us use some basic methods for some fundamental analytics.

- Count the characters of a text using the raw() method.
```
len(nltk.corpus.gutenberg.raw('shakespeare-hamlet.txt')
```
- Count the number of words using the words() method.
```
len(nltk.corpus.gutenberg.words('shakespeare-hamlet.txt')
```
- Count the number of sentences using the sents() method.
```
len(nltk.corpus.gutenberg.sents('shakespeare-hamlet.txt')
```

**Note:** The sents() method will require us to download the punkt file as discussed in Module 1.

- NLTK provides all these important methods for text analytics, although more advanced tasks may require to develop custom code.
- A common task is also to count the amount of vocabulary used in a file.
- In this case we extract all the words, then transform the words to a lower case list, and finally extract a set of the list.
- Converting data into a set can help us remove the duplicate values:
```
len(set([word.lower() for word in nltk.corpus.gutenberg.words('shakespeare-hamlet.txt')]))
```
- By analysing the data we conclude that the text includes 37,360 words, of which 4716 are unique words or punctuation symbols.
- Let us count the longest sentence in the book called Shakespeare Hamlet.
```
max([len(s) for s in nltk.corpus.gutenberg.sents('shakespeare-hamlet.txt')])
```
- It seems that the longest sentence contains 174 characters.

### Counting Vocabulary

- One of the most common tasks is to count the words of a natural language text.
- Let us use *text5: Chat Corpus*
```
import nltk
nltk.download('book')
from nltk.book import *
len(text5)
```
- This corpus has 45,010 words and punctuation symbols. These are known as *tokens*.
- We can extract the vocabulary of a text using a set datastructure. We can also sort it in order to get the data organised in alphabetical order.
```
sorted(set(text5))
```
- This command will print a list of all the vocabulary used in the chat corpus.
- Let us count how many unique words and punctuation symbols exist in out dataset.
```
len(set(text5))
```
- Although this corpus has 45,010 words and punctuation symbols, there are only 6,066 unique words.

### NLTK Simple Statistics

- Let us develop a small program to find the 20 most frequent words of the Chat corpus.
- A frequency distribution diagram will help us to find the frequent words:
```
fdist1 = FreqDist(text5)
fdist1.plot(20, cumulative=True)
```
- Let us use the dispersion_plot method. This reveals patterns in the word positions. Each stripe represents an instance of a word, and each row represents the entire text.
```
text5.dispersion_plot(['chat','JOIN','Player'])
```

 ### NLTK fine grained selection 
 
- Let us look for long words, for example, words with a length of 15 characters or more for *text9: The Man Who Was Thursday by G . K . Chesterton 1908*.
```
words = [word for word in set(text1) if len(word)>15]
sorted(words)
```
- Surprisingly, there are only two words: 'incomprehensible' and 'undenominational'.

### Running NLTK tasks

- Let's start working with the NLTK library.
- The following code will download a book collection that we can use as our dataset for learning NLP.
```
# The following script will download the books in our notebook for us to access
import nltk
nltk.download('book')
from nltk.book import *
```
**Note:** This code was previously used above but was not formely introduced until this section.

- We just downloaded a selection of texts, let's run the texts() script to see the book list:
```
texts()
```
- The above will print:
```
text1: Moby Dick by Herman Melville 1851
text2: Sense and Sensibility by Jane Austen 1811
text3: The Book of Genesis
text4: Inaugural Address Corpus
text5: Chat Corpus
text6: Monty Python and the Holy Grail
text7: Wall Street Journal
text8: Personals Corpus
text9: The Man Who Was Thursday by G . K . Chesterton 1908
```
- NLTK is a powerful language with a selection of tools to analyse data.
- Use the *concordance* method to search for the context that the word *feel* appears in *text6: Monty Python and the Holy Grail*:
```
text6.concordance('feel')
```
- The above will print:
```
Displaying 6 of 6 matches:
I can ' t take him . DEAD PERSON : I feel fine ! CUSTOMER : Well , do us a fav
can do ? DEAD PERSON : [ singing ] I feel happy ... I feel happy . [ whop ] CU
SON : [ singing ] I feel happy ... I feel happy . [ whop ] CUSTOMER : Ah , tha
AUNCELOT : Idiom ! CONCORDE : No , I feel fine , actually , sir . LAUNCELOT : 
ing sense . [ clap clap clap ] And I feel sure that the merger -- er , the uni
 s not quite dead . HERBERT : No , I feel much better . FATHER : You fell out 
```
- Use the similar method to extract words with a similar range of context with the word *person*, using *text5: Chat Corpus*:
```
text5.similar('person')
```
- This will print:
```
name u back boys day time way case list flavour end top truth sound
diary rights balad border price foothills
```
- Use the collocations method to extract phrases that are often used with another phrase in a way that sounds correct to people, Use *text6: Monty Python and the Holy Grail*.
```
BLACK KNIGHT; clop clop; HEAD KNIGHT; mumble mumble; Holy Grail;
squeak squeak; FRENCH GUARD; saw saw; Sir Robin; Run away; CARTOON
CHARACTER; King Arthur; Iesu domine; Pie Iesu; DEAD PERSON; Round
Table; clap clap; OLD MAN; dramatic chord; dona eis
```
- Let's count how many words are in *text6: Monty Python and the Holy Grail*.
```
print(len(text6))
```
- This will print 16,967.
- Count how many unique words and punctuation symbols exist in *text6: Monty Python and the Holy Grail*:
```
print(len(set(text6)))
```
- This will print 2,166.

### NLP Pipeline

- An NLP pipeline is a set of steps that allow us to perform basic analytics and build up a natural understanding software.
- Let's create a pipeline to break apart the following text found on the below website:
    - https://en.wikipedia.org/wiki/Athens

### Step 1: Segmentation

- Firstly, we break the text into sentences using the punctuation mark, so we can have the following:
    - Athens is the capital city of Greece.
    - Athens dominates and is the capital of the Attica region and is one of the world's oldest cities, with its recorded history spanning over 3,400 years.
    - Classical Athens was a powerful city-state.
- Sentence segmentation allows computers to process text easily in comparison to the whole text.
- Modern NLP pipelines use more sophisticated ways of segmentation, in order to make data more easy to work with.

### Step 2: Word Tokenisation

- The next step is to break the sentences into words we can process one at a time. For instance, "Athens is the capital and largest city of Greece", becomes, ""Athens","is","the","capital","and","largest","city","of","Greece"".
- English tokenisation is quite easy, as we can split the text whenever there is a space.
- The punctuation mark has a meaning (indicated at the end of the sentence) so we will need to keep it as a token.

### Step 3: Predicting Parts of Speech (POS) for Tokens

- Next step is to look for the part of speech of each token including:
    - Nouns, verbs, adjectives, adverbs, pronouns, prepositions, conjunctions, interjections ... etc.
- By understanding the structure of the sentence and the role of each word we can understand the meaning and the concept about the text.
- We can use a pre-trained part of speech model to classify words, for example:
    - Input -> Word: Athens surrounding words are "is" and "classic".
    - Part of speech classification model
    - Output: "Proper_Noun"
- This model is based on statistics, and it does not consider the meaning of the words.
- Extracting the POS we can start getting some basic understanding of the meaning of our sentence.
- For example, the nouns are:
    - Capital, City, Athens.
    - Athens is a proper noun, as it's a name used for the place (person or organisation).
    - Athens: PROPN, is: AUX, the: DET, capital: NOUN, and: CCONJ, largest: ADJ, city: NOUN, of: ADP, Greece: PROPN.

### Step 4: Text Lemmatisation

- All languages appear in various formats and forms.
- Let's examine the following sentences:
    - I bought a ball.
    - I bought two balls.
- Both sentences have a noun but using two different inflections.
- When working with data it's helpful to know the base form, so words with a similar meaning or concept can be identified.
- Lemmatisation refers to transforming verbs, nouns ... etc, to their roots.
- In our case, both sentences become:
    - I bought a ball -> I [buy] a [ball]
    - I bought two balls -> I [buy] a [ball]
- Let us examine how the lemmatisation works for our text:
    - Athens is the capital and largest city in Greece.
- A lemmatisation process will provide us the unconjugated form as follows:
- Athens: PROPN, is: AUX, the: DET, capital: NOUN, and: CCONJ, largest: ADJ, city: NOUN, of: ADP, Greece: PROPN.

### Step 5: Identifying Stop Words

- Next step is to identify the stop words or what we usually call filler words. For instance, "and", "the", "a", ... etc.
- Stop words removing allows us to isolate the important meaning of a text and remove the noise of unnecessary data.
- This is a common practice when we do statistics for NLP.
- Let us examine how our sentence is transformed after this step:
    - Input text: ["Athens","is","the","capital","and","largest","city","of","Greece","."]
    - Output text: ["Athens","capital","largest","city","Greece","."]. This is similar to speed reading, where we extract the required information and memorise key facts.

### Step 6: Dependency Parsing

- The goal is to build a tree that assigns a single parent word to each word in a sentence.
- This will help us figure out how all the words in our sentence relate to each other.
- This process is depicted by the diagram below:

<p align="center"> <img width="650" src= "/Diagrams/1.png"> </p>

### Step 7: Names Entity Recognition (NER)

- NER seeks to locate and classify name entities mentioned in unstructured text into pre-defined categories such as person names, organisations, locations, medical codes, time expressions, quantities, monetary values, percentages, ... etc.
- Let us see how a NER model transforms our text:
- *Athens (GPE)* is the capital and largest city of *Greece (GPE)*.
- The goal of NER is to identify and label key nouns with real-world concepts that they represent.
- In our case, an NLP model will be able to identify a GPE feature:
    - GPE is a Geopolitical entity, for example, countries, cities, and states.
- NER features include peoples' names, organisations, product names, dates and times, amounts of money, events, ... etc.

### Step 8: Coreference resolution

- This is the last step of our NLP pipeline.
- Using Coreference resolution we can identify parts of speech that are related with each other, especially those related with named entities.
- Let's examine the following example:
    - Athens is the capital and the largest city of Greece. It dominates the Attica region.
- Using Coreference resolution we can transform the text to the following:
    - *Athens* is the capital and the largest city of Greece. *It* dominates the Attica region.
    - *Athens* is the capital and the largest city of Greece. *Athens* dominates the Attica region.
- Coreference resolution is a challenging task and one of the most difficult steps in a pipeline. But recent research in deep learning has started making it highly effective.
- A common implementation of the coreference resolution is using neural networks.
- A good example is the https://huggingface.co/ where we can easily visualise our text and identify the relationship and similarities between words.

### NLP pipeline summary

- There are different ways of developing pipelines, and we will develop our pipelines using Python libraries.
- Different use cases require different NLP pipelines.
- However, the most common steps include the below:
    - 1.) Segmentation
    - 2.) Tokenisation
    - 3.) Part of speech
    - 4.) Lemmatisation
    - 5.) Stop words identification
    - 6.) Dependency Parsing
    - 7.) Name entity recognition
    - 8.) Coreference resolution

### Working with informal text using the Webtext corpus

- If we want to work with less formal text then the Guttenberg corpus, we can use the Webtext.
    - It includes text from forums, conversations, advertisements, ... etc.
    - Let us export the list using the following command:
```
from nltk.corpus import webtext
[id for id in webtext.fileids()]
```

- This will produce the following result:
```
['firefox.txt',
 'grail.txt',
 'overheard.txt',
 'pirates.txt',
 'singles.txt',
 'wine.txt']
```

 - Let's examine the pirates.txt file (Pirates of the Carribean: Dead man's chest!)
```
webtext.raw('pirates.txt')
```

- Let's run some basic analytics. In this example, we will count the occurence of each word in the pirates.txt file, excluding any stop words.
```
import nltk
nltk.download('stopwords')
allWords = nltk.tokenize.word_tokenize(webtext.raw('pirates.txt'))
allWordDist = nltk.FreqDist(w.lower() for w in allWords)
stopwords = nltk.corpus.stopwords.words('english')
allWordExceptStopDist = nltk.FreqDist(w.lower() for w in allWords if w not in stopwords)
```

- We can search now how many times a word "chest" appears in the dataset.
- There are 52 instances of this word in the text.
```
allWordExceptStopDist['chest']
```

- Let us run some basic analytics to find the top 10 words that occur more often in the dataset.
```
from collections import Counter
k = Counter(dic)
# Finding the 10 highest values
high = k.most_common(10)
for i in high:
    print(i[0], " :", i[1], " ")
```

### Working with the Brown corpus

- Brown corpus is an important dataset, usually used to study systemicatic differences between genres (stylistics).
- We can run a simple example to compare genres in their usage of modal verbs.

```
from nltk.corpus import brown
hobbies_text = brown.words(categories = 'hobbies')
fdist = nltk.FreqDist([w.lower() for w in hobbies_text])
modals = ['can','could','may','might','must','will']
for m in modals:
    print(m+": ", fdist[m])
```

- As expected, "will" is one of the most used words, showing that people talking about future ideas of hobbies.

### Working with the Reuters corpus

- Reuters corpus contains 10,788 news documents with a total number of 1.3 million words.
- The news have been classified by topics.
- There are 90 topics grouped into two sets:
    - Training set: The dataset we use to train an algorithm or model so it can accurately predict your income.
    - Testing set: The dataset to test the accuracy of a model using the training set.
- The following code downloads the Reuters corpus and shows the various categories:
```
import nltk
from nltk.corpus import reuters
nltk.download('reuters')
retuers.categories()
```

### Working with the Inaugural corpus

- Inaugural corpus is a collection of 55 texts, each text represents a presidential address.
- The following code demonstrates how to extract the Inaugural files:
```
from nltk.corpus import inaugural
nltk.download('inaugural')
inaugural.fileids()
```

### Annotated Corpora

- Text corpora include linguistic annotations:
    - Named entities
    - Syntactic structures
    - POS

- Examples include:
    - Brown Corpus: 15 genres, 1.15M words, tagged, categorised
    - Genesis Corpus: 6 texts, 200k words, 6 languages
    - Gutneberg (selections): 18 texts, 2M words
    - Inaugural Address Corpus: US Presedentual Inaugural Addresses (1789-present)
    - Reuters Corpus: 1.3M words, 10k news documents, categorised

### Working with Corpora in other languages

- There is a selection of languages supported by NLP, however, it might require some extra work in order to manipulate character codings.
- The following downloads and uses Spanish corpus:
```
nltk.download('cess_esp')
nltk.corpus.cess_esp.words()
```

- In this section, we have discussed different corpora including:
    - Gutenberg
    - Brown
    - Reuters
    - Inaugural

- Some of the corpora have an internal structure:
    - The Gutenberg is an isolated corpus with no particular organisation.
    - The Brown is categorised, for example by genre.
    - The Reuters is categorised, for example by news topic.
    - Inaugural represents data over time.

### Lexical resources

- A lexicon, or lexical resource, is a collection of words and/or phrases along with associated information such as part of speech and sense definitions.
- Lexical resources are secondary to texts, and are usually created and enriched with the help of texts.
- A lexical entry includes Headword (aka lemma), POS information, and Definitions.
- Two distinct words having the same spelling are called homonyms.
- Let us see the following example of homonyms:
    - "saw" (headword, or lemma) -> [verb] -> past tense of see (sense definition, or gloss)
    - "saw" (lexical entry) -> [noun] (part of speech or lexical category) -> cutting instrument

### Wordlist Corpora

- The simplest kind of lexicon with a sorted list of words.
- Very often we use wordlist to extract stopwords. It's a common task to identify stopwords to help us reduce the noise in our data. The following shows the stopwords in English:
```
from nltk.corpus import stopwords
nltk.download('stopwords')
stopwords.words('english')
```

- The following shows the stopwords in French:
```
from nltk.corpus import stopwords
nltk.download('stopwords')
stopwords.words('french')
```

### Wordnet Corpora

- WordNet is a large lexical database of English.
- Nouns, verbs, adjectives and adverbs are grouped into sets of cognitive synonyms (synsets), each expressing a distinct concept.
- WordNet superficially resembles a thesaurus, in that it groups words together based on their meanings.
- However, there are some important distinctions. First, WordNet interlinks not just word forms - string or letters - but specific senses of words.
- NLTK includes the English WordNet with 155.287 words and 117.659 synonym sets:
```
from nltk.corpus import stopwords
nltk.download('stopwords')
stopwords.words('french')
```

- Let's examine the following code:
```
import nltk
from nltk.corpus import wordnet as wn
nltk.download('wordnet')
wn.synsets('train')
```

- The word "train" has different meanings (synonym words or lemmas).
- We can extract definitions using the following code:
```
wn.synset('train.n.01').definitions()
```
- The word "train" has different meanings (synonym words or lemmas).
```
wn.synset('train.n.01').examples()
```
- Finally, let us see some hyponyms to extract more information from WordNet:
```
wn.synset('train.n.01').hyponyms()
```

### Introduction into Spacy

- Spacy is an NLP library specifically designed to help you run fast and efficient NLP tasks. It provides a selection of visualisations that can help us analyse natural language data.
- The following code renders a dependency model for a given text.
```
import spacy
from spacy import displacy
nlp = spacy.load("en_core_web_sm")
doc = nlp("Athens is the capital and largest city of Geece.")
from spacy import displacy
displacy.render(doc, style='dep', juptyer=True, options={'distance':90})
```

- The above will produce the following output:

<p align="center"> <img width="650" src= "/Diagrams/spacy.png"> </p>

### Summary

- Introduction to Natural Language Processing Corpora.
- Working with raw text.
- Introduction to Natural Language Processing theory.
- Word segmentation for different languages.
- Introduction to SpaCy library.

## Section 3: Information Extraction for NLP Tasks

In this section, we will cover:

- Introduction to information extraction (Regular Expressions).
- NLP visualisations.
- Bag of words and word vectors.
- Chunking and chinking.
- Word tagging.
- N-grams.

### Python Regular Expressions

- A regular expression (**regex**) is a sequence of characters that define a search pattern.
- Usually such patterns are used by string searching algorithms for "find" or "find and replace" operations on strings, or for input validation. For example, when a user inputs a telephone number.
- Regular expressions are the essence of data cleaning for textual data. They can help to solve parsing problems.
- Python has a built-in package called *re*, and makes regular expressions easy to use. Let us see a simple example:
```
import nltk
from nltk import re
text = "Mary is at home"
re.findall("Mary", text)
```
- The above code will print: ['Mary']
- Regular expressions are very powerful, let's see an example. Let's search the string to see if it starts with "Mary" and ends with "home".
```
text = "Mary is at home"
re.search("^Mary.*home$", text)
```
- Tokenisation is provided by NLTK, although we can still use regex to split at each white-space character:
```
re.split("\s", "Mary is at home")
```
- We can also replace white space characters with another character or number, for different tasks:
    - When you see "%20," it represents a space in an encoded URL.
    - The following code replaces a space with the "%20".
```
text = "Mary is at home"
re.sub("\s", "%20", text)
```
- Let us see the functions of the Python "re" module:
    - findall: Returns a list containing all matches.
    - search: Returns a Match object if there is a match anywhere in the string.
    - split: Returns a list where the string has been split at each match.
    - sub: Replaces one or many matches with a string.

- Metacharacters are characters with a special meaning, for instance:
    - []: A set of characters "[a-n]"
    - \: Signals a special sequence (can also be used to escape special characters) "\d"
    - .: Any character (except newline character) "he..o"
    - ^: Starts with "^hello"
    - "$": Ends with "world"$""
    - \*: Zero or more occurences "aix\*"
    - +: One or more occurences "aix+"
    - {}: Exactly the specified number of occurrences "a|{2}"
    - |: Either or "falls|stays"
    - (): Capture and group

- Let's see a more detailed example where we can extract a URL from a given text:
```
import re
text = """Web browsers request pages from web servers by using a URL. The URL is the address of a web page, like: https://www.w3schools.com."""
urls = re.findall('http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+',text)
print("Original string: ", text)
print("Urls: ", urls)
```

### NLP Visualisations

- Let's develop a program to find the 20 most frequent words of text1: Moby Dick by Herman Melville 1851.
```
import nltk
nltk.download('book')
from nltk.book import *
texts()
fdist1 = FreqDist(text1)
fdist1.plot(20, cumulative=True)
```

- Let us use the dispersion_plot method to reveal patterns in words positions. We will look for the words "chat", "JOIN", and "Player" using the text5 Corpus:
```
text5.dispersion_plot(["chat","JOIN","Player"])
```

### NLP Theory and Word Representations

- How to analyse text data in order to identify semantics of texts?
- Bag of words:
    - Using one hot encoding: Each word in the vocabulary is represented by one bit position in a huge vector.
- Let's examine the following text:
- My name is Bob, Hello world!
- In this vocabulary the word "name" can be represented as the following: 0 1 0 0 0 ...
- Processing text using this method does not utilise any contextual information.
- Word vectors:
    - Stores each word in a n-dimensional space where each point is represented by a vector of a specific dimensionality. Each dimension is a projection to a different axis.
- Let us examine the following text:
- My name is Bob, Hello world!
- In the vocabulary, the word "name" can be represented as the following: 0.3, 0.5, 0.02, ...
- Processing text using this method utilises contextual information.

### 
