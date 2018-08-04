# Twitter-Bot
A Twitter bot is a type of bot software that controls a Twitter account via the Twitter API. The bot software may autonomously perform actions such as tweeting, retweeting, liking, following, unfollowing, or direct messaging other accounts.

SETUP REQUIREMENTS
* First, I downloaded Tweepy. You can do this using the pip package manager(pip install tweepy),also you need python interpreter(i used 3.5 version)

CREDENTIALS

Next, we need to link our Twitter account to our Python script. Go to apps.twitter.com and sign in with your account. Create a Twitter application and generate a Consumer Key, Consumer Secret, Access Token, and Access Token Secret. Now you are ready to begin!

Under your import statements store your credentials within variables and then use the second block of code to authenticate your account with tweepy.

consumer_key = 'consumer key'
consumer_secret = 'consumer secrets'
access_token = 'access token'
access_token_secret = 'access token secret'

auth = tweepy.OAuthHandler(consumer_key, consumer_secret)
auth.set_access_token(access_token, access_token_secret)
api = tweepy.API(auth)
