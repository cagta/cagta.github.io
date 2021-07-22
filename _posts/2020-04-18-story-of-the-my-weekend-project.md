---
layout: post
title: story of the my weekend project!
---
this weekend, I coded two simple python tool for myself. it feels great when you accomplished this kind of things. I don't even remember when was the last time that I built this kind of satisfying side project. I think it is satisfying because it solves one of my problem.

I really like to ready articles about anything that triggers my curiosity. it includes bunch of things like history, psychology, business, economy, applied science and of cource computer science. so I have to reach out lot's of different resource to gather these article. they are mostly online web articles but sometimes I'm downloading pdfs, docs, epubs etc.

at the beginning, I was reading all of them on my computer and on my phone. I have to admit that it was mostly on my phone because I can carry it everywhere with me easily so that I can read it on bus, while waiting some friends etc. which means I can turn almost all of my idle time into productive entertainment.

however after a while my eyes start to complain. since I'm computer engineer, I'm always looking at screens when I added this idle times my eyes were really tired. after these complaints I discovered the e-ink technology and Amazon Kindle. e-ink is a amazing technology. for more detail about the technology, you should check [this](https://www.youtube.com/watch?v=Oqu1--AzM7U) but short explaination is you can read your digital contents on a digital screen which looks almost like real paper.

after all, why I'm telling these? this post should be about a tool that I coded right? here's the deal. everytime that I want to pick some cool contents to read on my toy, I have go and find that contents for me. basically, I have great list of RSS on my feedly for person or focused online news platform. and I'm also hanging aroud bunch of other sites to pick articles.

it's as consuming as reading. so want to cut that time to increase my reading time. I was start to think about it, since I'm developing some automation tools for others for money. I think I can use that logic to gain my time. it's leads me to [gather-my-news](https://github.com/cagta/gather-my-news).

I started very small. this simple script go [dev.to](https://dev.to) -which is one of my most visited site on daily scrapping- and gathers most popular articles on weekly basis.
It prepares a list of the articles for me so that I can check them easily without any distraction. I can easily check their title's to detirmine if there is anythin catchy or not and their systatics(likes and comments). it really like this for two reason. first, I'm directly accessing audince approved articles. second, I can see what I need without dealing with fancy side bars and graphics which are mostly nothing but distracting.

I'm planning to add [world economic forum's reports](https://www.weforum.org/reports) and [world Turkish business council's reports](http://www.dtik.org.tr/yayinlar) to my script as soon as possible.

I would like to stop writing now for this post with giving technologies that I used as conclusion. I know I only tell you about one simple tool maybe I can mention the other on my next post.

Ingredients of my tool:

- [Python](https://www.python.org/) as base programming language
- [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/) for proccesing html
- [urllib](https://docs.python.org/3/library/urllib.html) for handling url