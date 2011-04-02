    Author       : Zigang Xiao <zxiao2@illinois.edu>
    Last Updated : 04/01/2011
    Description  : As the document name indicates, this tutorial focus on
                   introducing git in a pragmatic manner and in my way.

Introduction
============

Source Code Management (SCM)
----------------------------
Imagine you are doing a course project. After you worked out a basic version
of your program, you save it in a folder named `project_1.0`.
After you add some features that you are not sure whether will be awesome
or useful, you keep the previous have another folder `project_1.1`.
Several days passed, your work directory is cluttered with project folders.
You found a bug, but you are not sure what version introduced it.
You are collaborating with others and both of you modified a file.
Your group member just throw USB disk that contains a tar ball of his version
to you and after you unzipped it, you found that it overwrote your
modification.

What if there is a tool that can help you manage your project?
It has at least of these functions:

* Keep track of different versions
* Can roll back to versions easily
* Provide merging scheme that help group members combine their work
* Users can retrieve files through the network

Roughly speaking, this is the core functionality of a [Source Code
Management](http://en.wikipedia.org/wiki/Source_Code_Management)
software, aka revision control.  CVS is probably the earliest SCM software.
Other SCM tools include SVN, mercury, bazzar, etc.  This tutorial will give a
very brief introduction on git. However, these tricks covers 80-90% of my use
of [git](http://git-scm.com).

git
---
What is git? The following definition is copied from <http://git-scm.com>:
> Git is a free & open source, distributed version control system designed to
> handle everything from small to very large projects with speed and
> efficiency.

The most attractive point of git to me is its fast speed.
Distributed style is also a great advantage of git.
However, I will not going to compare it with other tool because I want to be
to the point as soon as possible. So let's go!


