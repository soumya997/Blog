---
title: Update Click Once .Net Location
date: '2018-05-24'
draft: true
categories: Code
tags:
  - .Net
  - Click Once
author: Chris Stayte
authorImage: uploads/chrisstayte_profilepic.jpg
comments: true
share: true
type: post
---
I use ClickOnce everyday for several internal applications. Recently, I had to move the publishing website to a new host.

Here is how you can acheive a completely transparent move without annoying your users or forcing them to uninstall and reinstall the application.



First, you need to publish the deployment files on the new server. The deployment configuration is as follows :

Publishing folder : URL on the new server

Installation Folder : URL on the new server

Updates Folder : URL on the new server

Revision : last revision + 2 (very important)



Then you need to deploy a new version on the old server with an updates folder on the new server. This way, next time the application launches, it will get the new version from the new server, and voila. Here is the configuration for the last deployment on the old server :

Publishing folder : URL on the old server

Installation Folder : URL on the old server

Updates Folder : URL on the new server

Revision : last revision + 1 (very important)
