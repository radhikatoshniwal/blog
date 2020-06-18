---
title: "u/answer-reddit-bot"
date: 2020-05-01
description: "a bot that uses the gpt2 language model to answer questions on r/AskReddit"
tags: [gpt2,python,PRAW]
---
 A few days back, I came across the [gpt-2 language model by OpenAI](https://openai.com/blog/better-language-models/)
 and a very easy to use python package [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 gpt-2-simple allows you to download existing models and finetune them for easy text generation.
 The Python Reddit API Wrapper was used to get the submission titles from the subreddit and post comments on the same.
 Initially, when the bot did not have enough karma, the number of comment submissions through the API was limited to
 1 every 10 minutes,     but as soon as the bot gained enough karma (about 10) the limit was lifted. 
 The whole project was done on a google colab notebook that you may find [here](https://github.com/radhikatoshniwal/answer-reddit-  bot/blob/master/answerbot774.ipynb).
 The 774M model was used as it wasn't too large and did not yield texts that were too obscure and bot-like.
 With only a few lines of code, fairly impressive answers were generated. Here are a few of them:
 ![Comments](resources/_gen/images/post-1/1.jpg)
