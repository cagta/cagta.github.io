---
layout: post
title: seiatc - how I'm using python?
---
this article originally published on [medium](https://cagta.medium.com/seiatc-how-im-using-python-69a611ca6c5).

Welcome to my second post of Software Engineer In A Telecommunication Company series. If you didn’t check the first post yet. You can read it from this [link](/2021/software-engineer-in-a-telecommunication-company/).

Python is one the oldest member of my skill set. As you may already know that I’m not a tool fanatic. I don’t see any value on this. Programming Languages are the tools that we are using to solve our real life problems. We may like one of them more than others but benefiting from all is better. After this explanation you may see my stand clearly. I love Python, but this doesn’t stop me from seeing its disadvantages as well as advantages.

According to [official site](https://www.python.org/about/) _“Python is a programming language that lets you work more quickly and integrate your systems more effectively.”_ I think it provides what it’s proposing. If we were talking more technically, its one of the interpreted languages. Which means your code will be read and interpreted line by line.

I don’t want to dig into discussions like _‘Is Python fast enough ?’_, _‘Why you should use Python for this and not to use for that ?’_ instead I would like to mention that why it’s a good choice for our case.

<strong>Easy to Learn</strong>

Python has a very simple syntax. You may argue with me about indentations however if you check the numbers of python projects, we can say that there is lots of people who already adopted it. By the way, those people have very different backgrounds from high school teachers to bioinformatic engineers.

<strong>Collection of Libraries</strong>

As a software engineer, I like to see what stays under the hood. However when its come to building a complex systems, I don’t prefer to invent the wheel while there is a stable, accessible solution. Python has lots of libraries which ensure these expectations. Let’s take a look what I’m using frequently.

If you are dealing with network equipment, you need to deal with lots of IP math. **ipaddress** and **netaddr** libraries are very useful for these kind of operations. If it’s just a simple operations like checking IP version, IP validation etc. , I prefer built-in ipaddress library. But for more complex operations like assigning an IP from a specific subnet, checking subnet size according to topology etc. , netaddr is my choose. But instead of being a built-in library, netaddr is a BSD licensed third-party library that widely used in network address manipulation.

IP manipulations are only the beginning of our journey. Accessing network equipment and gathering information about this device as important as preparing an IP pooling without overlap. There is several different network equipment on the market. Even if I’m working for one of the vendors, I need to know that how to access other vendors’ devices and what kind of information is available on these devices for me. That information is critique especially on migrating from a third-party network.

For that information, I need to access these devices then process the available data. **netmiko/paramiko** libraries are very common within our team. To be honest, I don’t even care to compare them. I just used whichever presented in the project that I contribute. Since I only use them to establish ssh connections, I don’t think it’ll make any difference :)

When it’s come to gather and process these kind of data **textfsm** is my best friend. According to it’s documentation textfsm is a `Python module which implements a template based state machine for parsing semi-formatted text.`. Thanks to it we can easily parse and get related information from several different devices.

<strong>Wide Application Range</strong>

With the help of diverse libraries and core feature of the language you can use Python with a variety of the fields from embedding applications to web applications. Thanks to that we had a chance to build both web applications and simple terminal applications with the same team without shifting over technologies.

After all, I’m happy with Python for now. Let me know what’s your experience.