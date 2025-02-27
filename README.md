This Web Scraping & Text Analysis project utilizes Python library PRAW (Python Reddit API Wrapper) to retrieve and extract posts and comments from subreddits, Reddit API credentials from Reddit's Developer Portal is required to run PRAW. 

See full documentation here (https://praw.readthedocs.io/en/stable/).

By analysing the harvested text, we are hoping to organize, understand and gain additional insights from it. There are 4 major practice areas of **Text Analytics**:
1. Descriptive statistics
2. Document clustering
3. Document classification
4. Sentiment analysis

![image](https://github.com/user-attachments/assets/f2df683e-f40a-452b-9a36-d5f5f4921bcf)


**Preprocessing** is often neccessary for text analytics tasks. The process to clean is highly customizable and users will have to decide how much preprocessing is needed. Preprorcessing tasks includes:
- **Case normalization**
  - Convert all characters to the best case
  - You can do _case folding_, which is to make everything lower case
  - But I prefer _true-casing_, which take the type of word into account
    - Example: I Live in canada => i live in Canada
- **Tokenization**
  - Tokenization splits sentences into individual words (aka _**tokens**_). The common technique is to split on the whitespace and special charaters.
  - I used the python library _**nltk**_.
- **n-grams and skip-grams**
  - n-grams return sequences of n adjacent words. It provides context around words for some models.
- **Removing unwanted characters/numbers**
  - Example of stop-words: _**a, an, and, are, as, at, be, but, by, for, if, in, into, is, it, no, not, of, on, or, such, that, the, their, then, there, these, they, this, to, was, will, with.**_
  - Stopping is the process of removing common words. Stopping helps remove noise and increase the efficiency in the later analytic process.
- **Stemming and lemmatizing**
  - Stemming reduces words to their root form (i.e., _**kick**_ is the root form of **_kicker, kicks, kicked, kicking,_** etc.).
      - There are a few popular algorithms to choose from:
        - _**Porter**_ (most gentle)
        - _**Snowball**_
        - _**Lancaster**_ (most aggressive)
  - Lemmatization is the advanced version of stemming, it takes part of speech (POS) into account. For example, the word _meeting_:
    - get stemmed to _meet_ as a verb
    - get stemmed to _meeting_ as a noun
  - Compared to stemming, lemmatization is much slower, but performs more accurately.
- Spell checking
- Removing stop words
- Removing common and rare words

This project focuses on Sentiment Analysis and Descriptive Statistics, looking into r/wallstreetbets, who played a major role in the GameStop short squeeze that caused significant losses for a number of US hedge funds and short sellers for a duration of time in early 2021. 
In this project you will also find analysis of other interesting topics about philosophy, ethics, and religion. 

**Note**: The findings from this analysis may not reflect the views of the overall population, nor necessarily my own.

Special thank you to Instructor Bill Chao for teaching the course! 🙌  

Thank you for reading :)
