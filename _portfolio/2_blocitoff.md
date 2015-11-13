---
layout: post
title: Blocitoff
thumbnail-path: "img/blocitoff.png"
short-description: Utility Application with Rake Automation
---

{:.center}
![]({{ site.baseurl }}/img/blocitoff.png)

{:.center}
<a class="button" href="http://blocitoff-noel123iamme.heroku.com" target="_blank"><i class="fa fa-cloud"> Demo Site</i></a> <a class="button" href="https://github.com/{{ site.theme.github }}/blocitoff" target="_blank"><i class="fa fa-fw fa-github"></i> Source Code</a>

### Summary

Build a self-destructing to-do list application.

### Explanation

So Blocitoff was my first project where I had to figure out how to do most of it on my own.  Granted, this is a very simply project, but when the training wheels come off, it can be intimidating.  After reviewing the "user stories", I realized I've already done most of it in the prior project.

### Problem

|------------|-------------------|
| User Story | Difficulty Rating |
|:-----------|------------------:|
| As a user, I want to sign up for a free account by providing a user name, password and email | 2 |
|------------|-------------------|
| As a user, I want to sign in and out of Blocitoff | 2 |
|------------|-------------------|
| As a user, I want to see my profile page | 2 |
|------------|-------------------|
| As a user, I want to create multiple to-do items | 3 |
|------------|-------------------|
| As a developer, I want to seed the development database automatically with users and to-do items | 1 |
|------------|-------------------|
| As a user, I want to mark to-do items as complete and have them deleted | 3 |
|------------|-------------------|
| As a user, I want to see how many days remain before a to-do item is automatically deleted | 1 |
|------------|-------------------|
| As a user, my to-dos should be automatically deleted seven days after their creation date | 2 |
|------------|-------------------|

Wire Frames

![]({{ site.baseurl }}/img/blocitoff_home.png)

![]({{ site.baseurl }}/img/blocitoff_index.png)

### Solution

The first few items were easily copied from the foundation project, Bloccit.

1. User Sign Up
2. User Sign-in / Sign-Off
3. User Profile
4. Seeding data

Similar, to creating posts, added a model, view, and controller (MVC) to create "To-Do" items

Using Ajax, created ability to add/remove to-do items from the list.

The big new item was the ability to automatically remove to-do items after they've expired.  This is where I had to implement Rake automation.

### Results

A working, production web application

### Conclusion

The biggest lesson I was learning in this project was how to implement my project requirements from a UX stand-point.  I'm not a designer, but I felt I could've done a much better job making my application look nicer from a user perspective.  The program functions, but it's not very pretty.  I spent several days trying learn more about HTML/CSS to better style my site, but I had to decide not to get bogged down in the details, otherwise, I'll find myself behind on my apprenticeship.

{:.center}
<a class="button" href="{{ site.baseurl }}/4_portfolio.html"><i class="fa fa-hand-o-left"></i> Back to Portfolio</a>   <a class="button" href="{{ site.baseurl }}/portfolio/3_blocipedia/">Next project: Blocipedia <i class="fa fa-hand-o-right"></i></a>
