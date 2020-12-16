# datamining_twitterXmongodb
 Data Mining of tweets withe MongoDB and Twitter API

### Goal
**We want to be able to extract tweets based on one or several specific hastags from twitter to then analyse them.**

To achieve this goal we will use this jupyter notebook as a template and go through these steps:
* Install **MongoDB**
* Get your personal credentals from the **Twitter API**
* Select some **hastags** related to a current event
* Use the Stream API to **collect tweets** to create our dataset
* **Analyse** the collected tweets

#### Requirements
* Jupyter Notebook
* [pymongo](https://pymongo.readthedocs.io/en/stable/installation.html) (`pip install pymongo`)
* [tweepy](http://docs.tweepy.org/en/latest/install.html) (`pip install tweepy`)
* With [Twitter API](https://apps.twitter.com/),  [create a twitter application](https://developer.twitter.com/en/application/intent) and get your acess tokens / credentials (tuto: [Authenticate a Python Application with Twitter using Tweepy](https://www.digitalocean.com/community/tutorials/how-to-authenticate-a-python-application-with-twitter-using-tweepy-on-ubuntu-14-04))
-  The file `.keys.json` should look like this but with your tokens:

    ```javascript
    [{
        "consumer_key": "xxxxxxxxx",
        "consumer_secret": "xxxxxxxxx",
        "access_token": "xxxxxxxxx",
        "access_token_secret": "xxxxxxxxx"
    }]
    ```

#### Useful sources:
* [**Mining the Social Web, 2nd Edition by Matthew A. Russell**](https://www.webpages.uidaho.edu/~stevel/504/Mining-the-Social-Web-2nd-Edition.pdf) (really cool and detailed book for mining Twitter, Facebook, Linkedin, Google+, web pages, etc!)
* [twitter doc](https://developer.twitter.com/en/docs/tweets/filter-realtime/api-reference/post-statuses-filter) the API limits permit you to do the requests inside the boundaries of the API
* composition of a [twit object](https://developer.twitter.com/en/docs/tweets/data-dictionary/overview/tweet-object)