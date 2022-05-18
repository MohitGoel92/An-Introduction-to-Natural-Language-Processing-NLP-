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

Examples of NLP include Siri (Apple), Whatsapp, and Alexa (Amazon). So in essence, NLP is a software for speech recognition, language understanding and analysis, dialogs, and speech to text. In NLP, text is treated as raw data that is usually unstructured. For instance, a report, email, review or complaint. An NLP program analyses and presents results in an automated way. As NLP programs aim to perform tasks based on understanding human langauge, the program is able to exctract information from text.

NLP makes human to machine interactions easy.
- NLP is a way to support human to machine communication.
- Data mining: Identify hidden meaning and patterns of natural language data in an automated way.
- Information extraction: Extracting useful information from text such as names, locations, telelphone numbers ... etc.

Why is NLP important?

- Interpretation and manipulation of language is a kew challenge for modern industries.
- A lot of text data is generated daily, making automated analysis a key task.
- Human language understanding NLP tasks for:
  - Reading text
  - Writing text
  - Speaking text
  - Listening text

Obstacles to NLP
- Exploring the meaning and relationships of languages to cognition and meaning of text was always a challenging task for scientists.
- Understanding natural language is already a difficult task for humans, let along machines. This is because languages can have a very ambiguous nature. For instance, "You know Tom", and "You know Tom?".
- Personal styles and many different ways of expressions. For instance, "OK :)", and "OK :(".
- Many different languages and colloquial styles.

A simple NLP solution to a problem is categorising emails into "Inbox" or "Junk". This is performed by seeking particular words or a combination of words and probabilistically deeming it as useful or spam. The classification uses a large dataset of already labelled emails as a guide to categorising the new or incoming emails. Phrases like "best price", "cash bonus", "earn money", "you won £1 million" ... are all triggers that will classify the email as spam. This is also know as **Text Classification**.

NLP uses a Corpus as the basis of its analysis.

**Corpus:** A huge collection of written data. In our case of email classification, these are the emails that are already classified and labelled as spam or ham.

Below is a basic outline of an NLP task:
- Preparing the text data for analysis.
- Creating word dictionaries of words and frequencies.
- Feature extraction process.
- Training a classifier to predict class of new emails.

Data is constantly being generated, for instance, social media (Twitter, Facebook, Whatsapp ... etc). Common use cases of NLP include:

- Chatbots: Heavily used for businesses such as customer services. If you type in "Hello", the NLP program analysis the text and will reply "Greetings!". NLP is used to map text to meaningful insights capable of responsing to written commands. For instance, typing in a request and the system providing you with the required data.
- Sentiment Analysis: Here NLP identifies and classifies the emotions within a text using text analysis methods. For instance, understanding the reviews for a restaurant and whether they are positive or negative.
- Creditworthiness Assessment: A.I. algorithms analyse text and provide credit scores as predictive analytics for banks. Banks use alternative data sets for scoring potentual borrowers, for instance, social media posts, internet activity, and online behaviour. The takes the below process:
    - Mining the web for information on potential customers.
    - Analysing the data and providing assessments of the customers creditworthiness.
    - Banks use trained datasets that are prelabelled indicating the level of risk for a customer.
- Hiring and Recruitment: NLP is changing the way HR operate. Traditionally, recruiters need to review thousands of CV's for a single job post which can takes hours and hours of navigating emails. NLP can support this process by analysing candidate reports and scoring them against standard datasets. This provides indications for top candidates, removing bias and increasing diversity.
- Healthcare: 
