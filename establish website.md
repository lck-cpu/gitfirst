# 问题
1.linux编译安装怎么安装？  
2.编写的c可执行文件用不用给其可执行权限？  
3.域名可以直接绑定博客的IP吗？  
4.谷歌硬盘的域名更换为自己域名的大概原理是什么？可以用在github建站上吗？  

---------------------------------------------------------------------
# 我的建站过程
  我是通过虚拟机里的linux作为服务器，然后内网穿透，然后白嫖域名。  
  下面我将列出我遇到的问题：  
  1.在linux中部署服务器  
        同时安装了apache和nginx导致端口复用，删除了apache还是默认apache界面，原来默认源码在同一个文件夹/var/www html/index.html。**<big> 注意要学会这个命令查看开放端口的使用：`netstat -ntlp`</big>**  
    还有几个命令:重启系统：`reboot`。重启nginx服务：`service nginx start`。  
  2.内网穿透  
        需要先再在别人给你的隧道中绑定你的ip，然后在根据别人的教程操作别人给你的客户端。  
        **注意：要给ngrok文件可执行权限`chmod +x (ngrok)`括号里面的是要启动的客户端名称**  
  3.域名绑定  
        域名需要解析然后把你的域名与你的--公网ip--绑定。    
        **注意：如果你的公网IP是在国内不包括香港则需要备案**  
        当你的域名绑定多个IP后，浏览器访问后，又删除剩一个IP，浏览器会警告你，这个域名不安全，这时清除浏览器数据即可。  
# markdown的常用语法 
- 加粗加大 `**<big></big>**，*内容*是斜体`  
- 换行 `行末2空格 or 空一行 or <br>`
- 列表 - * +后要空一格。
- 代码 行代码用``中间写内容,代码块用``````中间写内容。  
<br> 
**<big>高级：</big>** $\color{red}{红色字}$
代码：` $\color{red}{红色字}$`


