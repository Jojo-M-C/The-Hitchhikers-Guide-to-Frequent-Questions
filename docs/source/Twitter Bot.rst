Twitter Bot
===========

Installation
--------

The easiest way to install the latest version from PyPI is by using `pip`_::

    pip install tweepy

.. _pip: https://pip.pypa.io/

1. create a directory and a virtual environment 

.. code:: yaml
    mkdir tweepy-bots
    cd tweepy-bots
    python3 -m venv venv

2. activate virtual environment and install tweepy

.. code:: yaml
    source ./venv/bin/activate
    pip install tweepy

3. create requirements.txt 

.. code:: yaml
    pip freeze > requirements.txt


4 common steps of Tweepy programs
--------

1. Import the tweepy package
2. Set the authentication credentials
3. Create a new tweepy.API object
4. Use the api object to call the Twitter API


Example
--------

This code will download the tweets in your home timeline and print their texts to the console. 

.. code-block :: python

   import tweepy

   auth = tweepy.OAuth1UserHandler(
      consumer_key, consumer_secret, access_token, access_token_secret
   )

   api = tweepy.API(auth)
   
   public_tweets = api.home_timeline()
   for tweet in public_tweets:
       print(tweet.text)


