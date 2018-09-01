---
title: Using Coder.com With Hugo
date: '2018-09-01'
draft: false
categories: Coding
tags:
  - Coder.com
  - Hugo
author: Chris Stayte
authorImage: uploads/chrisstayte_profilepic.jpg
image: /uploads/usingcoderwithhugo.png
comments: true
share: true
type: post
---
I hate having to setup my development environment over and over again. Today I am going to show you how to set it up once. Along with my theme of free resources, Coder.com is perfect for coding anywhere on anything. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/-uLJNGnh-5Y" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## **Installing Hugo on Coder.com**

Run this command in the terminal

``` console
go get -u github.com/gohugoio/hugo
```

Go to `root/go/src/github.com/gohugoio/hugo` and run a `build` command. Once this is done copy the hugo binary to `/usr/local/bin`

Now you can use the `hugo` command anywhere.

## Running Hugo Command

Create a `package.json` file. Inside put


```JSON
{
    "scripts": {
        "coder": "hugo server --bind='0.0.0.0' -p 3000 -b <URL HERE> --appendPort=false"
    }
}
```

Mine Looks Like 

```JSON
{
    "scripts": {
        "coder": "hugo server --bind='0.0.0.0' -p 3000 -b https://3000-dreamflammablegnu.cdr.co --appendPort=false"
    }
}
```
