---
title: ubuntu上的nginx配置笔记
date: 2019-05-18 05:11:39
tags:
  - nginx配置
  - ubuntu
categories: 
  - 技术
  - nginx
---

# 快速检测nginx配置是否有误
 
nginx -t  


# 重启等命令（两种）：

- 第一种  

systemctl start  nginx    (注意写法，nginx写在最后)  
systemctl reload nginx  
systemctl restart nginx  
- 第二种  

nginx -s  reload  
nginx -s  quit

# nginx默认的静态资源目录

默认静态网站跟目录  /etc/nginx/sites-available/default 中设置的 /var/www/html/index.nginx-debian.html

# nginx代理静态资源的相关的配置文件，在服务器中的位置和设置方式

- 目录 /etc/nginx/conf.d/ 目录中以conf结尾的所有配置文件，其中/etc/nginx/nginx.conf是默认配置文件，其内容中最后两行为


	  include /etc/nginx/conf.d/*.conf;  
      include /etc/nginx/sites-enabled/*;
	 
	 

---

# 其他问题
 
Nginx默认主页中文乱码，是因为位于 /var/www/html/中的index.nginx-debian.html 即H5文件本身缺少了字符集设置：
<meta charset="UTF-8">，配好字符集即可。

# ubuntu安装nginx参考链接

https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04








