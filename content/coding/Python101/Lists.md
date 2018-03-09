---
title: "Lists"
date: 2017-12-27T16:22:49-05:00
draft: false

image: "uploads/python101.png"
categories: [Code, Tutorial]
tags: [Python, Tutorial, Lists]
author: "Chris Styate"

type: post
---
Today we go over `Lists` in python and some built in functions and how they apply to them.

<!--more-->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HoHW6a5psgo" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

>
#### Instantiating A List
``` python
my_list = [1, 2, 3]
my_list2 = [2.3, 4.5, 6.2]
my_list3 = ["Chris", "Stayte", "Pyton"]
my_list4 = [1, 2.2, "Python"]
```
###### As you can see a list can contain any other data type as well as mutiple data types.

<br/>

>
#### Accesing List Variables
``` python
my_list = [1, 2, 3]
print(my_list[0])
# prints 1
print(my_list[3])
# prints an error: out of index
print(my_list[0:3])
# prints [1, 2, 3]
# You can use '3' here becasue it tells 
# python where to stop and doesn't include it.
```
###### Keep in mind that the beginning index of all lists start at `0`.
 
<br/>

>
#### List Functions
<br/>
Append
###### Add an item to the end of the list. `Equivalent to a[len(a):] = [x]`.
``` python
my_list = [5, 10, 15, 20, 25, 30]

my_list.append(35)

# [5, 10, 15, 20, 25, 30, 35]
```
<br/>
Clear
###### Remove all items from the list. Equivalent to `del a[:]`.
``` python
my_list = [5, 10, 15, 20, 25, 30]

my_list.clear()

# []
```
<br/>
Copy
###### Return a shallow copy of the list. Equivalent to `a[:]`.
``` python
my_list = [5, 10, 15, 20, 25, 30]

my_list_2 = my_list.copy()
my_list_2.append(35)

# my_list = [5, 10, 15, 20, 25, 30]
# my_list_2 = [5, 10, 15, 20, 25, 30, 35]
```
###### Lists are passed by reference. If you want an actual copy of the list use this function.
<br/>
Insert
###### Insert an item at a given position. The first argument is the index of the element before which to insert, so `a.insert(0, x)` inserts at the front of the list, and `a.insert(len(a), x)` is equivalent to `a.append(x)`.
``` python
my_list = [5, 10, 15, 25, 30]

my_list.insert(3, 20)

# [5, 10, 15, 20, 25, 30]
```
<br/>
Remove
###### Remove the first item from the list whose value is x. It is an error if there is no such item.
``` python
my_list = [5, 10, 15, 20, 25, 30]

my_list.remove(10)

# [5, 15, 20, 25, 30]
```
<br/>
Pop
###### Remove the item at the given position in the list, and return it. If no index is specified, `a.pop()` removes and returns the last item in the list. (The square brackets around the i in the method signature denote that the parameter is optional, not that you should type square brackets at that position. You will see this notation frequently in the Python Library Reference.)
``` python
my_list = [5, 10, 15, 20, 25, 30]

number = my_list.pop(3)
# number = 20
# [5, 10, 15, 25, 30]
```
<br/>
Reverse
###### Reverse the elements of the list in place.
``` python
my_list = [5, 10, 15, 20, 25, 30]

my_list.reverse()

# [30, 25, 20, 15, 10, 5]
```
 
<br/>

>
#### Getting the number of items in a list
``` python
my_list = [5, 10, 15, 20, 25, 30]

print(len(my_list))

# Prints 6
```