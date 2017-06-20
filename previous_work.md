# Predicting Personality From Twitter
Published: 2011 IEEE International Conference on Privacy, Security, Risk, and Trust, and IEEE Internatinal Conference on Social Computing
Author: Jennifer Golbeck, Cristina Robles, Michon Edmondson, Karen Turner - Unersity of Maryland

Goal: Present a method by which a user's personality can be accurately predicted through the publicly available information on their twitter profile.

Hyphotesis: Social media profiles can predict personality traits

Overview of the Experiment:
- Big Five Personality Inventory to 279 subjects in twitter application(to meassure accuaracy).
  - 45 questions version of the Big Five Personality Inventory based on [O. D. John. Big five inventory, 2000.]
- Using 2000 most recent tweets of same user in the previous experiemnt
  - tweets aggregated, quantified, and passed through a text analysis tool to obtain a feature set.
  - develop model that can predict factors to within between 11% and 18% of the actual values.

Data Collection:
1. From Tweet was collected
- Number of followers
- Number of following
- Density of social network
- Number of "@mentions"
- Number of replies
- Number of hashtags
- Number of links
- Words per tweet

2. Merge tweet in a single document per user
3. (79 features)Analyse using LIWC(Linguistic Inquiry and Word Count)- provides 81 different feautres of text in five categories:
  - Standard Cound: word counts, words longer than six letter, number of prepositions, etc
  - Psychological Processes: emotional, cognitive, sensory and social Processes
  - Relativity: words about time, the past, the future
  - Personal concerns: occupation, finalcial issues, health
  - Other dimmensiond: counts of various types of punctuation, swear words

In this paper they exclude Standard count and other dimmensions features to eliminate what is likely to be nouse on the type of text they have. Because the document is not coherent.The exceptions are that they included word count, words per sentence and swear word counts
4. (14 features) MRC Language Features.
5. Sentimental analysis of each user's tweets using diccionary that assigns words sentiment values of -1 and +1 scale, computed a score that was the average sentimetn score for all words used in their list of tweets/
