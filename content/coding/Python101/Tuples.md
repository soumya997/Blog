---
title: "Tuples"
date: 2018-01-13T10:45:40-05:00
draft: true

image: "uploads/python101.png"
categories: [Code, Tutorial]
tags: [Python, Tutorial, Tuples]
author: "Chris Stayte"

# Set your video id for
type: post
---
Let's learn what `Tuples` are and why they differ from lists...

<!--more-->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-EtfXvikR-s"frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

>
#### Instantiating A Tuple
``` python
empty_tuple = ()
tuple1 = (5,) # You need the comma
tuple2 = ("Chris", "Stayte")
tuple3 = (1, 2.2, "Python")
```
###### As you can see a tuple can contain any other data type as well as mutiple data types. Also look how unlike lists, tuples use parentheses instead of square brackets.

<br/>

>
#### Accesing Tuple Variables
``` python
my_tuple = (1, 2, 3)
print(my_tuple[0])
# prints 1
print(my_tuple[3])
# prints an error: out of index
print(my_tuple[0:3])
# prints [1, 2, 3]
# You can use '3' here becasue it tells 
# python where to stop and doesn't include it.
```
###### Keep in mind that the beginning index of all tuples start at `0`.
 
<br/>

>
#### Tuple Functions
<br/>
Max
###### Returns item from the tuple with max value.
``` python
my_tuple = (5, 10, 15, 20, 25, 30, 24, 19, 14, 9, 4)

print(max(my_tuple))

# 30
```
<br/>