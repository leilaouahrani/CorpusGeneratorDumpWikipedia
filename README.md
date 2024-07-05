# All-Languages-Corpus-Generator-with-Wikipedia Dump
This work is supported by the Ministry of Higher Education and Scientific Research in Algeria (Project C00L07UN100120180002)

Conception & Supervision: L. Ouahrani & D. Bennouar /  Contributor: Abdennour BenHamida.

This code allows to generation a corpus based on keywords related to the subject of the study, cleaned and ready to use and works with every language supported in Wikipedia. 
The corpus will be stored in a JSON file in the same path as the ".py" is running. The output contains:
- Corpus Name
- Words count: total number of words and different words
- Articles count: number of Wikipedia articles returned into the corpus
- Articles: a dictionary containing all the textual data returned stored as { Article's title: Content}

1- Requirments: 
- You may need to enable these two commands if your punkt isn't installed, once downloaded and installed nltk will work perfectly fine:
  #1- import nltk
  #2- nltk.download('punkt')
- Python 2.7 or later
- Internet connection
- At least 20mb of free storage

2- Libraries used:
- Wikipedia: API for wiki articles, installation is required (pip install Wikipedia or pip3 if it doesn't work)
- re. sub: a function that allows  delete portions of text that are or are not in the text
- word_tokenize: we use to tokenize (split) our texts into a list of words
- request exception to handle connection errors and timeouts
- sleep for time out exception handling
- langdetect: a tool that detects languages, so that we don't return any article that is not written in Arabic

3- How to use:
- Call the "BuildCorp" function with its two parameters:
  - Keywords: a string with arabic owrds describing your research or a subject
  - Nmae: name of the json file that will be created after generation
- The more keywords you insert, the bigger and more precise the corpus will be
 
 For further questions or inquiries about this code, you can contact l_ouahrani@univ-blida.dz
 
