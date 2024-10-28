+++
author = "kk"
title = "Setup record"
date = "2024-10-28"
description = "To record how to setup the Blog"
tags = [
    "setup",
]
categories = [
    "setup",
]
series = ["setup"]
aliases = ["setup"]
image = "pawel-czerwinski-8uZPynIu-rQ-unsplash.jpg"
+++

This article records how I setup the Blog with a Hugo theme. 
<!--more-->
**Refer to:**  
https://gohugo.io/getting-started/quick-start/  
https://space.bilibili.com/3546647648799599/search/video?keyword=hugo

## Prerequisites(Windows):
* Install Git;
* Install Go;
* Install Hugo extend version;
* Get a github account, and create a repo for the blog.(https://github.com/wujiaforward/wujiaforward.github.io)


## Commandline works(build the blog based on hugo-theme-stack/exampleSite):
**Note:** *I used GitBash for the flowing setup commandline works.*
1. hugo new site <folder_name_for_your_blog>
2. cd <folder_name_for_your_blog>
3. git init
4. git submodule add https://github.com/CaiJimmy/hugo-theme-stack.git <themes/hugo-theme-stack>  
   // maybe just don't need the <> part in a more simple way. Need to change the flowing steps, check later.
5. themes/hugo-theme-stack: cp -r archetypes/ assets/ data/ i18n/ images/ layouts/ config.yaml <folder_name_for_your_blog>
6. themes/hugo-theme-stack/exampleSite: cp -r content/ hugo.yaml .gitignore <folder_name_for_your_blog>
7. hugo server -D  
   // check if the setup is OK
8. deploy the blog with githubpages. (https://gohugo.io/hosting-and-deployment/hosting-on-github/)
