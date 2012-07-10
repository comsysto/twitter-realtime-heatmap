twitter-realtime-heatmap
========================

A real-time Twitter heatmap as described on http://blog.comsysto.com/2012/07/10/real-time-twitter-heat-map-with-mongodb/


To get this running you need to have a few things:


* Twitter Streaming API credentials (which you need to enter in tstream.py)
* MongoDB
* a capped collection in MongoDB named "tweets_tail"
* Flask
* Redis
* Tweepy



First, start mongod and redis. Then start tstream.py, incoming tweets are logged to stdout. Then start tweet_service.py and connect your browser to http://localhost:5000/static/map.html and wait for the heatmap to form!
