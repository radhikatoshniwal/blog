---
title: "somebody-make-this"
date: 2021-01-30
description: "a random idea generator"
tags: [flask,firebase,heroku,html,css,python]
---
## What is this?\
[This](http://somebody-make-this.herokuapp.com/) is a random idea generator.\

## Why did I make this?\
I've been an active reddit user (almost too active, seriously though, need to tone down a little) for the past 2 years
and every now and then I stumble across a new subreddit and I wonder where it had been my whole life. One such subreddit was r/SomebodyMakeThis - a community where people 
who do not have the time, resources or skills share ideas they think are useful and need to be built. So I decided to scrape 2000 of these ideas and create a random idea generator out of it.\
I've been wanting to try Flask for a really long time and this project seemed like a simple project to start with.

## How did I make this? (a basic overview)\
1. I scraped the subreddit and stored the data in a Firebase. [Here's](https://github.com/radhikatoshniwal/Scraping-Subreddits/blob/main/Scraping_Subreddits.ipynb) the code for it.\
2. Designed a basic one pager using html+css.\
3. Created a flask app. I followed the [Flask by Example tutorial](https://realpython.com/flask-by-example-part-1-project-setup/) for this step. \
4. Now, added the one pager HTML file to a 'templates' folder within your working directory and the css file to a 'static' folder.\
5. In the app.py folder I imported the packages flask, random and firebase-admin. Please please make sure every time you install a package you do it in a virtual environment and keep adding it to your requirements.txt file. It will make your deployment process smoother.\
6. Added the Firebase API call to my application. Checkout my [html one pager](https://github.com/radhikatoshniwal/somebody-make-this/blob/main/templates/onepager.html) + my [app.py](https://github.com/radhikatoshniwal/somebody-make-this/blob/main/app.py) to see how I did it. 
7. Deployed it on Heroku and WE DONE HERE. [Follow this for the deployment process](https://devcenter.heroku.com/articles/github-integration).

## What did I learn?\
1. Notice how I said 'Please please use a virtual environment'. Yes, I learnt the importance of a virtual environment the hard way. Because I didn't use one, I ended up with a bunch of dependencies on my requirements.txt which I had to remove manually :'( \
2. I also learnt that you can build almost anything you want to because the internet is full of resources. It wasn't much of a revelation but just wanted to put it out there incase you're not starting a project that you always wanted to just because you aren't very familiar with the tech stack required for the project yet. I think the best way to learn in to just start and take baby steps as you go. 
