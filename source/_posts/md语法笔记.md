---
title: md语法笔记
date: 2019-05-17 22:34:23
tags:
  - markdown语法
---
  
# 一、md语法教程
[md语法教学链接](https://segmentfault.com/markdown)  

## 二、常见语法
- **分割线**可以使用三个减号；
- 如果需要在段落内加入**换行**，可以在前一行的末尾加入至少两个空格
- **超链接->    **[超链接按钮名]（超链接地址）
- 图片，即为超链接之前带一个感叹号! [GitHub] (https://avatars2.githubusercontent.com)
- 行内代码 英文状态下的斜点包住即可`func(){}` 
- 区块代码 段落前后各一个空行，每空行三个```  第一个空行可加上javascript等表示语言

// 下面是mysql的
update mysql.user set password = password('lin135531') where user = 'lcx' and host = '%';
grant all privileges on mysql.* to lcx@'%' identified by 'lcx';
*79211EB85AE483FFB8EB4FACF0A299E85EE1D0E7


update user set authentication_string=password('1111') where user='lcx';