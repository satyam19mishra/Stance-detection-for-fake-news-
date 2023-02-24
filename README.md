# Stance-detection-for-fake-news-
The goal of the Fake News Challenge is to explore how artificial intelligence technologies, particularly machine learning and natural language processing, might be leveraged to combat the fake news problem. We believe that these AI technologies hold promise for significantly automating parts of the procedure human fact checkers use today to determine if a story is real or a hoax.

# FORMAL DEFINITION
# Input
         A headline and a body text - either from the same news article or from two different articles.
# Output
         Classify the stance of the body text relative to the claim made in the headline into one of four categories:
         Agrees: The body text agrees with the headline.
         Disagrees: The body text disagrees with the headline.
         Discusses: The body text discuss the same topic as the headline, but does not take a position
         Unrelated: The body text discusses a different topic than the headline

# Flow Diagram for the dataset
![image](https://user-images.githubusercontent.com/103360091/221267717-986465e4-21dd-4272-a6f1-e71abe1cb74a.png)

# About Dataset
   # Context
The issue of “fake news” has arisen recently as a potential threat to high-quality journalism
and well-informed public discourse. The Fake News Challenge was organized in early
2017 to encourage development of machine learning-based classification systems that
perform “stance detection” -- i.e. identifying whether a particular news headline “agrees”
with, “disagrees” with, “discusses,” or is unrelated to a particular news article -- in order to
allow journalists and others to more easily find and investigate possible instances of “fake
news.”

   # Content
The data provided is (headline, body, stance) instances, where stance is one of {unrelated, discuss, agree, disagree}. The dataset is provided as two CSVs:

   # train_bodies.csv
This file contains the body text of articles (the articleBody column) with corresponding IDs (Body ID)

   # train_stances.csv
This file contains the labeled stances (the Stance column) for pairs of article headlines (Headline) and article bodies (Body ID, referring to entries in train_bodies.csv).

   # Distribution of the data
The distribution of Stance classes in train_stances.csv is as follows:

          rows	unrelated    discuss	 agree        disagree
          49972	0.73131	    0.17828	0.0736012     0.0168094
There are 4 possible classifications:

    The article text agrees with the headline.
    The article text disagrees with the headline.
    The article text is a discussion of the headline, without taking a position on it.
    The article text is unrelated to the headline (i.e. it doesn’t address the same topic).
