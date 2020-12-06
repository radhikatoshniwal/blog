---
title: "u/answer-reddit-bot"
date: 2020-05-01
description: "a bot that uses the gpt2 language model to answer questions on r/AskReddit"
tags: [gpt2,python,PRAW]
---
 A few days ago, I came across the [gpt-2 language model by OpenAI](https://openai.com/blog/better-language-models/)
 and a very easy to use python package [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 that allows you to download existing models and finetune them for easy text generation.
 So, I thought it'd be fun to play around with it and see how it'd respond to some of the questions on r/AskReddit. I set up [this](https://www.reddit.com/user/answer-reddit-bot) account and registered my app [here](https://ssl.reddit.com/prefs/apps/) under the same. Be sure to register it as script.
 I used The Python Reddit API Wrapper to get the submission titles from the subreddit and post comments on the same.
 Initially, when the bot did not have enough karma, the number of comment submissions through the API was limited but this gets lifted as soon as the account gains about 10 karma.
The whole project was done on a jupyter notebook that you may find [here](https://github.com/radhikatoshniwal/answer-reddit-bot/blob/master/answerbot774.ipynb).
I used the 774M model as it wasn't too large and did not yield texts that were too obscure and bot-like.
 With only a few lines of code, fairly impressive answers were generated. Here are a few of them:
 
 ![1image](https://i.imgur.com/yxXTPBL.jpg)
 ![2image](https://i.imgur.com/SDAmWCB.jpg)
 ![3image](https://i.imgur.com/WlRKc5A.jpg)
 ![4image](https://i.imgur.com/astMPK7.jpg)
 ![5image](https://i.imgur.com/mtU5Awf.jpg)
 This was a fun little project and a lot of people did not realise they were talking to a bot despite the username being a dead giveaway. People on the internet  would really just engage with anyone(or anything)! 
 My account got banned from r/AskReddit but that's okay because such is life!
 You, however, may checkout more comments [here](https://www.reddit.com/user/answer-reddit-bot)!
 
