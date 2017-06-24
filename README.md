# Goal
Predict personality traits (Big 5 factors) using style markers features extracted from tweets

# Motivation
Currently we are surrounded by ai systems like siri, alexa which are doing a great
job on interacting with the user to some functionalities like: call someone,
schedule appointments and son on; but they like on customized interaction.

Every ai has its on way of responding and creating sentences that later are
translated into sounds using text-to-speech techniques. But the reality is that
every person has a different reaction to the writing style of the agent giving a
response. Every sentences has an emotion related and every one is more identified
with different ways of writing.

In order to create an ai that responds in a ways that the user will find likeable
we need first to identify the map personalities to understand what personalties we
like and the suggest a better sentence structure for the ai to have a more human
interaction with the user.

This project try to identify personalities of tweeter user using the writing style
as a first stage project

# Methodology
The framework purposed to meet the goal has four steps: Data Collection, Features Extraction, Model Building and Results Evaluation.

## Data Collection
Data was retrieved from a public database released by Twitter for research purpose on year 2014 containing infomation about tweets. In this research we only are going to use two dimensions of this dataset cointaining the twitter id(user) and tweet(body).

The raw dataset contains over 700GB containing 665,246,249 observations in different languages. Each instance has information about: location, tweet text,  so first users related to Entrepenuership and Startups were selected as target users for the experiments. To select this users Twitter API was used to get more information about the user and be able to filter user that are related to this field

Then the tweets text was preprocessed to remove messages that don't provide value for the learning and testing. For the purpose of this research the following filters were applied:
1. Tweets that contains quotes were removed because don't represent a writing style of the user.
2. Re-Tweets were removed
3. Stop list
4. Users that has more than 1000 tweets.
5. Tweets in english language
6. Users related to companies or accounts that are used for marketing purposed were removed

After the preprocessing we end up with a clean dataset of independent users from the domain related to Entrepenuership and Startups that has tweets in english, not re-tweets or quotes. This is the dataset used for the following experiments.


## Features Extraction

## Model Building


## Results Evaluation

### Personality Insight Watson

# Modules

- PersonalityPredictor
  Detects 5 personality factor base on: structure of sentences, frequent words

# Results
