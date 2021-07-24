---
layout: post
title: seiatc - how I'm using git?
---
Welcome to my third post of Software Engineer In A Telecommunication Company series. If you didn’t check the previous posts yet, check the links below. 

* [software engineer in a telecommunication company](/2021/software-engineer-in-a-telecommunication-company/)
* [seiatc - how I'm using python?](/2021/seiatc-how-im-using-python/)

My main objective is experimenting with ideas with Git. Anytime I want, I can easily create a branch and work on my new ideas without breaking the existing codebase. I prefer to use `git checkout -b newBranchName`. It is like a combination of `git branch newBranchName` and `git checkout newBranchName`. After that, I directly jump on the code and try my ideas.

Sometimes I come up with another solution while coding the other one. At that time, I am using `git stash` to remove all unstaged changes. This command lets me start over and save the current changes. I am using this store as a shelf of possible solutions. `-m` flag let you write notes about your stash. If you want to remember what is going on with that version of the changes, I strongly suggest using it. But let's be honest, most of the time, we are skipping that :) At least, Git keeps track of our stashing with a number. Keep in mind, it is working like a stack. The first stashed changes place at the bottom of the list.

Let's dig into another use case. In an ideal world, we should have a development and commit plan before starting to code. I will be honest with you. Mostly it is not the case. The problem looks too easy to solve then you start typing. Just a couple of minutes later, you notice your assumption is wrong. After that minute, you start coming back and forth while trying to enhance your solution. You can guess how this will affect your commit history.

`git rebase -i` is probably my favorite command. You can divide your commits into smaller chunks, can edit their messages, and can rewrite your whole commit history. I like this feature and widely use it. However, I am only using it if the branch that I am working on is not public. When you use rebase, it will change your commits' hashes. If you are working on a public one, this means disaster for your colleagues. So be careful about it.

Before closing, I would like to mention some valuable resources that can enhance your Git knowledge.

* [Simplify writing code with deliberate commits](https://www.youtube.com/watch?v=mE8DZUfhdm4&list=PLTmfDkA8k73yOWuLROLvtYOI1ipj4PNi8&index=7)
    * It suggests 5 practical habits which will make your commits more deliberate.

* [A Branch in Time](https://tekin.co.uk/2019/02/a-talk-about-revision-histories)
    * A talk about the revision history.

* [How GitHub Uses GitHub to Build GitHub](https://www.youtube.com/watch?v=qyz3jkOBbQY)
    * It is probably the oldest resource that I am sharing with you. But there are still valuable and valid bits of advice in it. On the other hand, do not let the title misleads you. You will find valuable information about Git.

* [Git tip: committing with verbose mode](https://tekin.co.uk/2020/03/git-commit-verbose-mode)
    * After I discover verbose mode, I never looked back.

`Self Marketing Warning!! The following article is mine. So I can not be objective about it. :)`
* [git tag; lightweight or annotated?](/2021/git-tag-lightweight-or-annotated/)
    * Let's you decide which type of tag is more useful for your case.