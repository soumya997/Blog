---
title: "Strings"
date: 2017-11-25T15:08:20-05:00
draft: false


categories: [Code, Tutorial]
tags: [Python, Tutorial, Strings]
author: "Chris Stayte"
image: "uploads/python101.png"
type: post
---

Today we look at what strings are and how we create them in python.

<!--more-->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KquuQ-YWU3I" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

>
#### Single Quote String
``` python
my_string = 'This is my string'
```
#### Double Quote String
``` python
my_string = "This is my string"
```
#### Multi Line String
``` python
my_string = ''' This is my
multi line string. It can span
mutiple lines which makes it great
for formatting output or keeping
the code clean.'''
```
#### Using Quotation Marks In A String
You can do this mutiple ways. Here are two.
``` python
version1 = "These are single quotes 'words'"
# print(version1) -> These are single quotes 'words'

version2 = "These are double quotes \"words\""
# print(version2) -> These are double quotes "words"
```
If you look at the code you can see that using the opposite quotes allows you to use
them in the string. If for some reason you have to use the same type of quote to
encase the string as well as in the string you can 'escape' the quotes using the
forward slash. This tells python not to interpret the quotes and to keep them as 
their literal context of a character.
