---
layout: post
title: summary of devops readings
---
some of you may already know, while I'm trying learn something new, I like to dig in multiple resources to see different aspects of it and prepare a summary from all of them. with that way I believe I'm learning way better and sharing this knowledge makes me feel like, I'm giving back to community.

today, we are gonna talk about DevOps. before writing this summary DevOps was a frequently heard trending topic for me. I thought it was just a new field at software world. I was seeing vacancies which are titled as DevOps Engineer alongside with several discussions about DevOps like tool comparisons, role/responsibility sharing etc. besides that, I was feeling like I'm just seeing the results instead of the needs and the starting point of this trendy topic. we are talking about DevOps since late 2008. there are several definitions of DevOps, I will try to give the most convincing one for me. 

let's start with Dev of DevOps. we can say that every thing we do for building our softwares is Dev side of DevOps; designing, coding, testing etc. after creating softwares we should run them without any trouble in a designated place with acceptable performance. everything we do to ensure that can be seen as Ops part of DevOps; monitoring, incident management, maintainence, performance evaluation etc. another definition can be this: Dev is the people who are involved with building software and Ops is the operations needed while building, testing, maintainining/providing services. 

all of these explanations are both wrong and right. they are right because all of these are some part of DevOps. but they are also wrong because DevOps means unification of the concepts not separation of them. "DevOps is defined by people building software and how they work together, not simply by what’s in their toolchain." [[1]](https://github.blog/2020-10-07-devops-definition/)

so why do we need to unify these concepts? because, we want to ship our softwares faster than ever without sacrificing stability and security. thing about google, facebook, github or any other company you see as a pioneer of the software world. the conditions and the expectations of the world is changing rapidly. no one tolerate 1 hour denial of service anymore. in critical system, even minutes can be seem unacceptable. this is not new. but the thing is world expecting you to deliver that quality within days or months not within years. while you are providing security and stability, there is always a new feature to be discovered or introduced. pioneers want to be either innovators or early adopters [[2]](https://en.wikipedia.org/wiki/Technology_adoption_life_cycle). even being an early majority may be considered as failure.

<img src="https://upload.wikimedia.org/wikipedia/en/4/45/DiffusionOfInnovation.png">

while we are facing such a big demand there is no way except unifying all the stakeholders of the process. for me this is what DevOps is. All the things which let us work more closely than before to produce stable, secure and efficient softwares. All the stakeholders should be aligned and be aware of each other's way of work.

<img src="/assets/images/posts/2021-01-03-devops.png">

I took the figure above from Andrew Clay's presentation [[3]](https://youtu.be/IdCnYNmpB44?t=1919) I believe it's is great in terms of showing the whole concept of DevOps. 

finally, after giving brief information about the DevOps. I encourage you to dig in the details of resources that I follow while writing this post.

**resources**
- [What is DevOps? A guide to common methods and misconceptions](https://github.blog/2020-10-07-devops-definition/)
- [Getting started with DevOps automation](https://github.blog/2020-10-29-getting-started-with-devops-automation/)
- [The evolving role of operations in DevOps](https://github.blog/2020-12-03-the-evolving-role-of-operations-in-devops/)
- Andrew Clay SHAFER's [Closing Keynote - Elemental DevOps](https://www.youtube.com/watch?v=IdCnYNmpB44&list=PLTmfDkA8k73yuhx2tutvnayp6xjxO-4C9) at DevOpsDays Istanbul 2018 
- Andrew Clay SHAFER's [Closing Keynote](https://www.youtube.com/watch?v=k2zpLNIjpBI) at DevOpsDays Istanbul 2019 

**references**
- [1] [https://github.blog/2020-10-07-devops-definition/](https://github.blog/2020-10-07-devops-definition/)
- [2] [https://en.wikipedia.org/wiki/Technology_adoption_life_cycle](https://en.wikipedia.org/wiki/Technology_adoption_life_cycle)
- [3] [https://youtu.be/IdCnYNmpB44?t=1919](https://youtu.be/IdCnYNmpB44?t=1919)