---
layout: post
title: Building Skynet - Machine Learning
---

So there's this topic called "Machine Learning," and it's been getting a lot of attention in the press over the past several years. Maybe you've heard of it (or maybe you're already a world-renowned expert in it, in which case thank you for visiting my blog but I don't think this post is for you :) ). Startups and tech giants alike have flaunted their machine learning technology for better valuations and PR wins. Here are some examples:

* http://www.businessinsider.com/facebook-facial-recognition-technology-ai-cant-see-face-2015-6
* http://venturebeat.com/2016/01/27/googles-ai-beats-a-professional-go-player-an-industry-first/
* http://www.cnn.com/2012/04/09/tech/inside-netflixs-popular-recommendation-algorithm/index.html
* https://www.pehub.com/2015/11/paxion-leads-20-mln-funding-of-h2o-ai/
* https://techcrunch.com/2016/02/19/salesforce-acquires-predictionio-to-build-up-its-machine-learning-muscle/

... and the list goes on and on. You'll notice several of those articles talk about "deep learning," an especially hot topic in machine learning these days, but we'll get to that later. So what is machine learning? How does a machine "learn"? Are we really on the verge of an [artificial](http://www.dailymail.co.uk/sciencetech/article-2931375/Bill-Gates-says-fear-robot-uprising-Microsoft-founder-says-agrees-Elon-Musk-dangers-AI.html) [intelligence](http://www.vanityfair.com/news/2016/06/the-one-technology-that-terrifies-elon-musk) [apocalypse](http://www.bbc.com/news/technology-30290540)? This series of posts will dive in to what machine learning is in general and then will dig into various machine learning algorithms, tips and tricks, with code samples included. It may even delve into some philosophical musings on AI's impact on humankind's fate. In honor of these afore-linked modern-day geniuses/prophets of the ai-pocalypse, we'll call this series of posts on machine learning "Building Skynet."

## Teaching Machines

How does a machine "learn"? What does it even mean for a machine to learn? Understanding that is going to take a little bit of statistical background.

Machine learning is essentially a game of pattern recognition. Humans are really good at pattern recognition. Just for fun, try finding the patterns in these examples:

What's the next number in this sequence: 1,2,4,8,16,?

That was too easy. Name the next number in this sequence: 1,1,2,3,5,8,13,21,?

How about this one: 1,14,91,364,1001,?

Kudos if you got the last one, it's pretty arcane compared to the other two. These patterns have something in common - they are all perfectly predictable. There is an underlying function that generates each number in the sequence such that you can get the exact right answer to the question "find the nth number" every time as long as you know the underlying function. Unfortunately, in the real world almost nothing is perfectly predictable. There is no mathematical function (at least that we know of) to perfectly predict the price of a given stock at any given time, for example. But even though the world around us is not perfectly predictable, there are clearly patterns around us. Take, for example, this chart:

![alt text](http://www.mathresources.com/products/insidemath/figures/scatpl02.png)

