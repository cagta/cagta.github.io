---
layout: post
title: localhost while vpn is on?
---
As a developer, I'm always looking for ways to improve my development environment. To be honest, I'm too lazy to repeat silly manual operations again and again. And today I'm gonna share one of my way of doing that.

Since I'm a corporate guy, while I'm away from my office I'm using our corporate VPN. Why I'm repeating this corporate thing again and again because when you are in such a big company you mostly have very limited space to change things in your favor. For example, in this case, I have to divide my internet traffic into two separate parts. The traffic that needs to be going on a VPN and the traffic that needs to be going on my localhost.

I need that because, in default, if you are using VPN it means the local network was changing. So if you had a virtual machine which is running on your local pc like mine, it will become inaccessible since your local network was changed.

I overcame this situation by using the port forwarding feature of the Oracle VirtualBox. With the help of that now I can access all of my services which is actually on my virtual machine.

Even the one image will tell you the story which can be seen below. Go to your network settings of you Virtual Machine then add one NAT interface to your machine and at the advance option of this interface add some port mappings like below. And here we go. Now we can access the webserver which is being served over port 80 of the virtual machine and accessible on port 8080 of my host. 

<img src="/assets/images/posts/2020-04-10-ayvmwctv-oracle-virtual-box.png">