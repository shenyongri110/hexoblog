---
title: Building A Website With Hexo
date: 2016-10-21 17:31:25
tags: Hexo
categories: Hexo
---

# Starting
I have tried many website building frameworks , but "Hexo" is really easy to set up and use. Today, let's study how to build and configure a simple website by using the magic "Hexo". I think it is a good start for biginner and we will give an example by using NexT theme which is a precise and popular framwork.
![](/images/hexo-setup-01.png)
<!--more-->

# Content
This artical is just for Windows user.

## Install Git
The official installing method is available for download on the Git website. Go to http://git-scm.com/download/win and download will start, click the exe file until finishing installation.

## Install NodeJs
Go to the NodeJs official website https://nodejs.org and you will find the installing packages for different systems, just choose Windows version and download. Here we have two choices to install which are ".msi" and ".exe". Either of them can be executed on Windows platform.

## Install Hexo
First of all, we need to realize some commands of hexo.

```bash
$ hexo g #completed command is "hexo generate" which is used for generating static file.
$ hexo s #completed command is "hexo server" which is used for starting the server.
$ hexo d #completed command is "hexo deploy" which is used for deploying local files onto github.
$ hexo n #completed command is "hexo new" which is used for creating a new post.
```

Right-click anywhere on the desktop and select Git Bash, then execute the follow command
```bash
$ npm install hexo-cli -g
```

If we come across the error below
```bash
ERROR Deployer not found : github
```

We can execute the following commands first
```bash
$ npm install hexo-deployer-git --save
$ npm g
$ npm d
```

Then we need to create a folder that is for placing blog project, for example, "E:\hexo". Enter "E:\hexo" and right-click, we also select Git Bash and execute commands. Hexo will generate all files the website needs.
```bash
$ hexo init
$ hexo install
```

For now, we can see what files hexo generate, just execute commands
```bash
$ npm g
$ npm s
```

Visit http://localhost:4000/ in the browser, there will be a fine webpage. So now we have built a local website successfully.
![](/images/hexo-setup-02.png)
