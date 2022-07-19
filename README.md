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
- 

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

- NLP programs heavily or linguistic datasets knows as **corpora**.
- A corpus is a collection of texts using in machine learning tasks.
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

