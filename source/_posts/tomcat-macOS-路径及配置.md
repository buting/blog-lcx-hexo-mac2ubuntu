---
title: tomcat-macOS-路径及配置
date: 2019-05-06 10:09:16
tags:
categories: 
  - 技术
  - tomcat
---
macOS 环境下的tomcat的默认存储位置-using homebrew
<!--more-->

### tomcat包储存路径 ↓

    /usr/local/Cellar/tomcat@8/8.5.38/libexec
    (cellar是酒窖或者地下室的意思，这样你懂了吧，存储各种应用的地方)


### tomcat访问路径 ↓

    /usr/local/opt/tomcat  
    tomcat -> ../Cellar/tomcat/9.0.10  
    tomcat@8 -> ../Cellar/tomcat@8/8.5.38  
    tomcat@9 -> ../Cellar/tomcat/9.0.10
    (软链接到了上文的存储路径)