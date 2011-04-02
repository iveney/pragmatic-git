    Author       : Zigang Xiao <zxiao2@illinois.edu>
    Last Updated : 04/01/2011
    Description  : As the document name indicates, this tutorial focus on
                   introducing git in a pragmatic manner and in my way.
                   I try to introduce the most useful functions of git
                   as concise as possible.

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
very brief introduction on [git][git]. However, these tricks covers 80-90% of
my use of git.
Note that this tutorial [itself][pragmatic-git] is managed with the help of git.

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

Git Basics
==========
Installing git
--------------
Git is available in various platform.  The easiest way it to install it using
the corresponding package manager in your OS, e.g., yum in Fedora Linux,
apt-get in Ubuntu, homebrew in Mac OS X.  For Windows, please refer to
<http://git-scm.com>.
Alternatively, you can build git from source.

Making a Git repository
-----------------------
Now let's say you want to create a project `hello` that will be written in C.
You need to create a directory for it and cd into it first:
    $ mkdir hello
    $ cd hello
You then initialize this directory:
    $ git init
You should see the output `Initialized empty Git repository in ...`,
where `...` is your directory location.

Adding things to the repository
-------------------------------

Git Branching
=============

Working with Remote Repository
==============================

Tips and Tricks
===============
Interactive and partial adding
------------------------------
Debugging using git
-------------------
Picking a single commit
-----------------------
GUI
---

Further Reading
===============
[Pro Git][progit] is probably the best free book of introducing git.

Final Words
===========
Now you are good to go!
If you want some project to train your git skill before you deploy in
real work, you can just go to [github][github] and `fork` the project
for this document: [pragmatic-git][pragmatic-git].
Try to translate this document to your language then
send a `pull` request to [me][iveney].
During the translation, use git to manage your work.

Happy gitting!

[git]:    http://git-scm.com    "git"
[github]: http://github.com     "Github"
[pragmatic-git]: https://github.com/iveney/pragmatic-git   "pragmatic-git"
[iveney]: https://github.com/iveney     "iveney"
[progit]: http://progit.org/book/       "progit"
