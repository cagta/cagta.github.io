---
layout: post
title: git tag; lightweight or annotated?
---
this article originally published on [medium](https://cagta.medium.com/git-tag-lightweight-or-annotated-43bf52888835).

>_<strong>TLDR;</strong> use annotated tags that contain tagger name, email, date, and message. In that way, you can isolate taggers from commit authors. You can see who tagged which commit. Otherwise, you would have just the author of the commit. You can also secure them with a GPG sign. On the other hand, lightweight tags are just simple pointers. You may prefer to use them privately to put a pinpoint on your commit history._

Git has two different tag types: lightweight and annotated. At first sight, you may think there is no problem using them interchangeably. However, the git commands like 'git describe' take annotated tags by default. Of course, you can use related flags and bypass this behavior like 'git describe - tags'. However, let me show you why you may prefer annotated tags over the lightweight ones. The most common scenario for using tags is releasing a new version.

Consider this scenario, you are a newbie in a team of 10 developers. Somehow you need to investigate one of the older versions of your project because of a problem at production. And you saw that this code should not ship in the first place. At that time, you may want to be sure about your judgment. so who should you talk to? This is where things get interesting. If the release tag is lightweight, you will see something like this.

```bash
$ git show v1.4
commit ca82a6dff817ec66f44342007202690a58967412
Author: Cagatay Tanyildiz <cagta@mail.com>
Date:   Fri 25 21:52:11 2021 -0300
   
   Change version number
```

Which is quite unclear who made that tagging? Yes, you can still see the author of a specific commit. But do you remember all of the auditors of your codes? I don't think so. So the first advantage of annotated tags is detailed information which is absent in lightweight tags and isolating the tagger of the commit from the author of the commit. In that way, you can see who made this commit and who tagged it as a valid production commit.

Let's think of another way. You built a Jenkins pipeline that takes all the tags from your repository and changes production code each time it detects a release tag. If you built your system on top of lightweight tags, you should think twice. How you are traceback your release even if you are not sure who approved it? Again, author/auditor isolation is needed.

Lastly, you may have a customer who wants to ensure that they pull in a verified set of changes onto their platforms. In that case, you need to GPG sign each of your release tags. This is only applicable to annotated tags because of their information storing capacity. More specifically, they contain the tagger name, email, date, and the message. Also, they can be signed with GPG. check 'Whodunnit for paranoid people' section of this article for detail. An annotated tag will look like this.

```bash
$ git show v1.2
tag v1.2
Tagger: Cagatay Tanyildiz <cagta@mail.com>
Date:   Fri 25 22:12:11 2021 -0300

version 1.2
commit ca82a6dff817ec66f44342007202690a58967412
Author: Cagatay Tanyildiz <cagta@mail.com>
Date:   Fri 25 21:52:11 2021 -0300

    Update location list
...
```

In conclusion, you should use annotated tags by default which have more detail than lightweight tags, even if you are not sharing them with others. Otherwise, you can neither see the tagger nor sign it when you need it.